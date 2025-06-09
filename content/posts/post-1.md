---
title: "Javascript Operators for beginners"
description: "programming operators"
date: 2025-06-09
image: "/images/posts/jsoperators.jpg" 
categories: ["programming"]
authors: ["Evatitan"]
tags: ["Javascript", "operator"]
draft: false
---

Programming operators are essentials for our daily coding activities. When I first started learning a programming language, I found it difficult to remember all the English terms, so I even took a maths course on Udemy to help me become more familiar with the symbols. While this was helpful, programming operators are not the same as mathematical symbols. Therefor I share this article with you in the hope that it will help you.

## Operators list

| Symbol         | Name                          | Description                                      |
|----------------|-------------------------------|--------------------------------------------------|
| `+`            |  Addition                     | Adds two values together  |
| `-`            |  Subtraction                  | Subtract two values |
| `*`            |  Multiplication               | Multiples two values           | 
| `/`            |  Division                     | Division of two or more values          |
| `%`            |  Modulo (remainder)           | Returns the remainder after dividing of two values |
| `**`           |  Exponentiation (ES6)         | Raises a value to the power of N            |
| `++`           |  Increment                    | Adds 1 to a value every time             |
| `--`           |  Decrement                    | Subtracts a value by 1 every time            |
| `=`            |  Assign                       | Assign a value to a variable           |
| `+=`           |  Add and assign               | Adds the value on the right to the variable on the left, then assigns the result back to the variable on the left |
| `-=`           |  Subtract and assign          | Subtracts the value on the right from the variable on the left and assigns the result back to that variable             |
| `*=`           |  Multiplication and assign    | Multiplies the value on the right by the variable on the left and assigns the result back to that variable             |
| `/=`           |  Division and assign          | Divides the value on the right by the value on the left and assigns the result back to the variable on the left            |
| `%=`           |  Modulo and assign            | Returns the result of the modulo operation between two values and assign it back to the variable            |
| `**=`          |  Exponentiation assign        | Raises a variable to the power of a value and assigns the result back to the variable.             |
| `==`           |  Loose equality               | Compares two values to see if they are equal          |
| `!=`           |  Loose inequality             | Compares two values to see if they are not equal              |
| `===`          |  Strict equality              | Compares two values and their type if they are equal           |
| `!==`          |  Strict inequality            | Compares two values and types if they are not equal           |
| `>`            |  Greater than                 | Returns the result of the comparison if the left value is greater than the right one          |
| `<`            |  Smaller than                 | Returns the result after comparing if the left value is smaller than the right one             |
| `>=`           |  Greater and equality         | Returns the result after comparing if the left value is greater or equal than the right one           |
| `<=`           |  Smaller and equality         | Returns the result after comparing if the left value is smaller or equal than the right one              |
| `&&`           |  AND                          | Returns true only when both sides are true        |
| `\|\|`         |  OR                           | Returns true when one side is true               |
| `!`            |  NOT                          | Returns the contract value           |
| `? :`          | Ternary (conditional)         | Returns the first value if the condition is true; otherwise, returns the second value.            |
| `&`            | Bitwise AND                   | Performs AND on each bit of two numbers          |
| `\|`           | Bitwise OR                    | Performs OR on each bit of two numbers           |
| `...`          | Spread/rest                   | Expands or collects elements/arguments           |

### Examples
<details>
<summary>Show Addition Example</summary>
```js
let a = 5;
let b = 3;
let result = a + b; // result is 8
console.log(result);
```
</details>

<details>
<summary>Show Subtraction Example</summary>
```js
let a = 5;
let b = 3;
let result = a - b; // result is 2
console.log(result);
```
</details>

<details>
<summary>Show Multiplication Example</summary>
```js
let a = 5;
let b = 3;
let result = a * b; // result is 15
console.log(result);
```
</details>

<details>
<summary>Show Division Example</summary>
```js
let a = 9;
let b = 3;
let result = a / b; // result is 3
console.log(result);
```
</details>

<details>
<summary>Show Modulo Example</summary>
```js
let a = 9;
let b = 3;
let result = a % b; // result is 0
console.log(result);
```
</details>

<details>
<summary>Show Exponentiation Example</summary>
```js
let a = 9;
let b = 3;
let result = a ** b; // result is 729
console.log(result);
```
</details>

<details>
<summary>Show increment Example</summary>
```js
let a = 9;
let result = a++; // result is 9
console.log(result);
```
</details>

<details>
<summary>Show decrement Example</summary>
```js
let a = 9;
let result = a--; // result is 9
console.log(result);
```
</details>

<details>
<summary>Show assign Example</summary>
```js
let a = 9;   // result is 9
console.log(result);
```
</details>

<details>
<summary>Show Add and assign Example</summary>
```js
let a = 9;
a += 1; // this is equal to [a = a + 1],  a is 10
console.log(a);
```
</details>

<details>
<summary>Show Subtract and assign Example</summary>
```js
let a = 9;
a -= 1; // this is equal to [a = a - 1],  a is 8
console.log(a);
```
</details>

<details>
<summary>Show Multiplicate and assign Example</summary>
```js
let a = 9;
a *= 2; // this is equal to [a = a * 2],  a is 18
console.log(a);
```
</details>

<details>
<summary>Show Division and assign Example</summary>
```js
let a = 9;
a /= 3; // this is equal to [a = a / 3],  a is 3
console.log(a);
```
</details>

<details>
<summary>Show Modulo and assign Example</summary>
```js
let a = 9;
a %= 3; // this is equal to [a = a % 3],  a is 0
console.log(a);
```
</details>

<details>
<summary>Show Exponentiation and assign Example</summary>
```js
let a = 9;
a **= 3; // this is equal to [a ** 3],  a is 729
console.log(a);
```
</details>

<details>
<summary>Show Loose equality Example</summary>
```js
let a = 9;
let b = "9";
console.log(a==b);  // true
```
</details>

<details>
<summary>Show loose inequality Example</summary>
```js
let a = 9;
let b = 8;
console.log(a!=b);  // true
```
</details>

<details>
<summary>Show Strict equality Example</summary>
```js
let a = 9;
let b = "9";
console.log(a===b);  // false
```
</details>

<details>
<summary>Show Strict inequality Example</summary>
```js
let a = 9;
let b = 8;
console.log(a!==b);  // true
```
</details>

<details>
<summary>Show Greater than Example</summary>
```js
let a = 9;
let b = 8;
console.log(a > b);  // true
```
</details>

<details>
<summary>Show Smaller than Example</summary>
```js
let a = 9;
let b = 8;
console.log(b < a);  // true
```
</details>

<details>
<summary>Show Greater and equal Example</summary>
```js
let a = 9;
let b = 9;
let c = 8;
console.log(a >= b);  // true
console.log(a >= c);  // true
```
</details>

<details>
<summary>Show Smaller and equal Example</summary>
```js
let a = 9;
let b = 9;
let c = 8;
console.log(b <= a);  // true
console.log(c <= a);  // true
```
</details>

<details>
<summary>Show ADD Example</summary>
```js
let a = true;
let b = false;
console.log( a && b );  // false
```
</details>

<details>
<summary>Show OR Example</summary>
```js
let a = true;
let b = false;
console.log( a || b );  // true
```
</details>

<details>
<summary>Show NOT Example</summary>
```js
let a = true;
console.log(!a);  // false
```
</details>

<details>
<summary>Show Ternary Example</summary>
```js
let a = true;
let b = 1;
let c = 2;
let result = a ? b : c
console.log(result); 
```
</details>

<details>
<summary>Show Ternary Example</summary>
```js
let a = true;
let b = 1;
let c = 2;
let result = a ? b : c
console.log(result); 
```
</details>

<details>
<summary>Show Bitwise AND Example</summary>
```js
let a = 5;  // binary: 0101
let b = 3;  // binary: 0011
let result = a & b;  // result is 1 (binary: 0001)
console.log(result);  // Output: 1
```
</details>

<details>
<summary>Show Bitwise OR Example</summary>
```js
let a = 5;   // binary: 0101
let b = 3;   // binary: 0011
let result = a | b; // result is 7 (binary: 0111)
console.log(result); // Output: 7
```
</details>

<details>
<summary>Show Spread/Rest Example</summary>
```js
let a = [1,2,3]
let b = [...a, 4 , 5] // b is [1, 2, 3, 4, 5]
console.log(b);
```
</details>



## Others Operators List

<details>
<summary>Show List</summary>

Here are some additional common JavaScript operators

| Symbol         | Name                          | Description                                      |
|----------------|-------------------------------|--------------------------------------------------|
| `^`            | Bitwise XOR                   | Performs XOR on each bit of two numbers          |
| `~`            | Bitwise NOT                   | Inverts each bit                                 |
| `<<`           | Bitwise left shift            | Shifts bits to the left                          |
| `>>`           | Bitwise right shift           | Shifts bits to the right                         |
| `>>>`          | Bitwise unsigned right shift  | Shifts bits to the right, filling with zeros     |
| `typeof`       | Type determination            | Returns the type of a variable                   |
| `instanceof`   | Instance check                | Checks if object is an instance of a constructor |
| `delete`       | Delete property               | Removes a property from an object                |
| `void`         | Void                          | Evaluates expression and returns undefined       |
| `new`          | Object instantiation          | Creates an instance of an object                 |
| `in`           | Property existence            | Checks if property exists in an object           |

</details>
