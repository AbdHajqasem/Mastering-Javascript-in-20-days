# Day12
## Philosophy of Coercion:

You don't deal with these type conversion corner cases by avoiding coercions. 

Instead, you have to adopt a coding style that makes value types plain and obvious

A quality JS program embraces coercions, making sure the types involved in every operation are clear. Thus, corner cases are safely managed. 

JavaScript's dynamic typing isnot a weakness, it's one of itsstrong qualities

![image](https://github.com/AbdHajqasem/Mastering-Javascript-in-20-days/assets/122126568/4bcd0b3f-b863-43fd-b0e9-44befafc0c26)

![image](https://github.com/AbdHajqasem/Mastering-Javascript-in-20-days/assets/122126568/bd1b4b7d-6ec4-4458-bb8e-c10c399d1d6e)

### Coercion Exercise:

**tests:**

![image](https://github.com/AbdHajqasem/Mastering-Javascript-in-20-days/assets/122126568/cc72e6f4-06c9-479e-aae7-bad11dbf3c0e)

---
![image](https://github.com/AbdHajqasem/Mastering-Javascript-in-20-days/assets/122126568/839ce6f7-afa9-4798-92f3-0561c0afe4f0)


![image](https://github.com/AbdHajqasem/Mastering-Javascript-in-20-days/assets/122126568/cd720eda-e6c8-4054-92d7-bd4584af9c3a)

![image](https://github.com/AbdHajqasem/Mastering-Javascript-in-20-days/assets/122126568/225d2215-08bd-41bc-a1be-505ecf11dbed)

---

## Equality:

**'==' Vs. '==='**:

![image](https://github.com/AbdHajqasem/Mastering-Javascript-in-20-days/assets/122126568/7143ac35-f8b1-4847-aab2-c3406504e34d)

![image](https://github.com/AbdHajqasem/Mastering-Javascript-in-20-days/assets/122126568/6664ea07-6299-4920-986c-22b9c7460a8a)

![image](https://github.com/AbdHajqasem/Mastering-Javascript-in-20-days/assets/122126568/97beb8a1-3aed-48e1-8ef0-a2feaad0db15)

![image](https://github.com/AbdHajqasem/Mastering-Javascript-in-20-days/assets/122126568/a6c68218-ecdc-44e6-b5a9-1d3119dd71d7)

z![image](https://github.com/AbdHajqasem/Mastering-Javascript-in-20-days/assets/122126568/3e523f59-f9da-456f-b82a-6cc7ed48dd1e)

### Coercive Equality:

![image](https://github.com/AbdHajqasem/Mastering-Javascript-in-20-days/assets/122126568/b59fb682-af24-468a-891b-dcdf54e2561e)

### Double Equals Alogorithm:

![image](https://github.com/AbdHajqasem/Mastering-Javascript-in-20-days/assets/122126568/a2e14000-017d-405d-97ba-51d124a150c6)

![image](https://github.com/AbdHajqasem/Mastering-Javascript-in-20-days/assets/122126568/ab93a396-956d-4658-9b85-0780bd1ea528)

![image](https://github.com/AbdHajqasem/Mastering-Javascript-in-20-days/assets/122126568/25142524-60c0-42b4-86b1-a69a57c7ed92)

**Explain** 

![image](https://github.com/AbdHajqasem/Mastering-Javascript-in-20-days/assets/122126568/3eeb3c40-745f-470c-ace9-8c7b7cd6700e)

**Summary:**

If the types are the same: ===

If null or undefined: equal 

If non-primitives: ToPrimitive Prefer: ToNumber

---

### '==' corner cases:

![image](https://github.com/AbdHajqasem/Mastering-Javascript-in-20-days/assets/122126568/b21ffea7-c643-40a9-a864-91bb64f0233c)

**Explain** 

![image](https://github.com/AbdHajqasem/Mastering-Javascript-in-20-days/assets/122126568/06434b51-7ad9-4f31-a082-4ccc251bd535)

**with booleans**

![image](https://github.com/AbdHajqasem/Mastering-Javascript-in-20-days/assets/122126568/48431ca1-ace6-40a8-a502-10e2e6bd46ac)

**never do  '==' with true or with false**

**Explain** 

![image](https://github.com/AbdHajqasem/Mastering-Javascript-in-20-days/assets/122126568/cf0b99ad-31c7-4be8-859c-09401d46b896)

**how to avoid**:

![image](https://github.com/AbdHajqasem/Mastering-Javascript-in-20-days/assets/122126568/3ed96677-c122-4ec8-af0b-1b830ed8db75)

---
### The case for double equals:

Knowing types is always better than not knowing them +tatic Types is not the only (or even necessarily best) way to know your types 

![image](https://github.com/AbdHajqasem/Mastering-Javascript-in-20-days/assets/122126568/2dc3cf9a-af0c-4150-aa6c-d265e6446794)

![image](https://github.com/AbdHajqasem/Mastering-Javascript-in-20-days/assets/122126568/eb37f428-7398-4f47-ba6f-026bc6e05e94)

**Since === is pointless when the types don't match, it's similarly unnecessary when they do match.**

![image](https://github.com/AbdHajqasem/Mastering-Javascript-in-20-days/assets/122126568/16d88ba9-9a34-418e-8869-0ed1ef3d3032)

![image](https://github.com/AbdHajqasem/Mastering-Javascript-in-20-days/assets/122126568/ae90f7de-5f0f-4e53-801a-aff4bed8eccb)

![image](https://github.com/AbdHajqasem/Mastering-Javascript-in-20-days/assets/122126568/5bace2e1-d67f-40e3-8acc-2ef5ed622b87)

![image](https://github.com/AbdHajqasem/Mastering-Javascript-in-20-days/assets/122126568/b9c73cde-9ab3-4a02-a941-3cdb1922c4e0)

![image](https://github.com/AbdHajqasem/Mastering-Javascript-in-20-days/assets/122126568/e2ba9467-dada-426a-8a7b-8c82a68a12ab)

![image](https://github.com/AbdHajqasem/Mastering-Javascript-in-20-days/assets/122126568/8672aaed-c59b-4350-af7c-67a0bd75454a)

![image](https://github.com/AbdHajqasem/Mastering-Javascript-in-20-days/assets/122126568/71f54969-3048-4509-93b3-ba2dc57467f1)

---

![image](https://github.com/AbdHajqasem/Mastering-Javascript-in-20-days/assets/122126568/c059e1c0-aea7-4618-8fe9-1bbb47fcfe02)

**Tests**:

![image](https://github.com/AbdHajqasem/Mastering-Javascript-in-20-days/assets/122126568/ee21dcc2-6509-408e-8c61-72e48f693ab6)


**Answer**:

```javascript
function findAll(match,arr) {
  var ret = [];
  for (let v of arr) {
    if (Object.is(match,v)) {
      ret.push(v);
    }
    else if (match == null && v == null) {
      ret.push(v);
    }
    else if (typeof match == "boolean") {
      if (match === v) {
        ret.push(v);
      }
    }
    else if (typeof match == "string" && match.trim() != "" && typeof v == "number" && !Object.is(-0,v)) {
      if (match == v) {
        ret.push(v);
      }
    }
    else if (typeof match == "number" && !Object.is(match,-0) && !Object.is(match,NaN) && !Object.is(match,Infinity) && !Object.is(match,-Infinity) && typeof v == "string" && v.trim() != "") {
      if (match == v) {
        ret.push(v);
      }
    }
  }
	return ret;
}

function setsMatch(arr1,arr2) {
	if (Array.isArray(arr1) && Array.isArray(arr2) && arr1.length == arr2.length) {
		for (let v of arr1) {
			if (!arr2.includes(v)) return false;
		}
		return true;
	}
	return false;
}
```
---
## Static Typing:

### TypeScript & Flow:










  

































































