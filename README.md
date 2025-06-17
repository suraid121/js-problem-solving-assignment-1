# JavaScript Basic Problem Solving
## Problem Sheet 1 :
###  1. Create a variable called `carName`, assign the value `Volvo` to it.
##### Solution (js) :
```javascript
let carName = "Volvo";
```
### 2. On one single line, declare three variables with the following names and values.
##### Solution (js) :
```javascript
let firstName = "John" , lastName = "Doe" , age = 35 ;

```
### 3. Use the correct assignment operator that will result in x being 50 (same as x = x * y).
##### Solution (js) :
```javascript
let x = 10 , y = 5;
x = x * y;
console.log(x); // 50
```
### 4. Use comments to describe the correct data type of the following variables.
##### Solution (js) :
```javascript

let length = 16; // number type data
let lastName = "Johnson"; // string type data 

const a = {
  firstName: "John",  
  lastName: "Doe"
};    // object type data
```
### 5 . Execute the function named myFunction.
##### Solution (js) :
```javascript
 ( function myFunction() {
    alert("Hello World!");
  }) ();
// Connect js to html to see the result.
```
### 6. 3. Create an object called person with name = John, age = 50, Then, access the object to alert("John is 50").
##### Solution (js) :
```javascript


 const person = {
    name: "John",
    age: 50
 };
 
    alert(`" ${person.name}   is  ${person.age}" `);

// Connect js to html to see the result .

```
### 7. The <button> element should do something when someone clicks on it. Try to fix it.
##### Solution (html) :
```html
  <button onclick="alert('Thanks for clicking me')" > Click me </button>

```
### 8. Array Related Question 
#### 1. Alert the number of items in an array, using the correct Array property.
##### Solution (js) :
```javascript
const cars = ["Volvo", "Jeep", "Mercedes"];
   alert(cars.length); // 3
```

#### 2.  Change the first item of Brand to "Ford".  
##### Solution (js) :
```javascript

   const Brand = ["Volvo", "Jeep", "Mercedes"];
Brand[0] = "Ford"; 
console.log(Brand); //  ["Ford", "Jeep", "Mercedes"]

```
### 9. Math Related Problems
#### 1. Use the correct Math method to create a random number.
##### Solution (js) :
```javascript


let randomNumber = Math.random();
console.log(randomNumber) // it will give a random number .
```
#### 2.  Use the correct Math method to return the largest number of 10.
##### Solution (js) :
```javascript

 let maxNumber = Math.max(10,20)
 console.log(maxNumber) // 20

```
#### 3. Use the correct Math method to get the square root of 9.
##### Solution (js) :
```javascript
let squareRoot = Math.sqrt(9);
console.log(squareRoot) // 3
```
### 10. comparison operator related problems!
#### 1.  Choose the correct comparison operator to alert true, when x is greater than y. 
##### Solution(js) :
```javascript

let  x = 10 , y =5;
if(x > y){
    alert("true")
}else{
    alert("false")
}
// true
```
#### 2. Choose the correct conditional (ternary) operator to alert "Too young" if age is less than 18, otherwise alert "Old enough".


##### Solution(js) :
```javascript 
let age = 19;
let message = age < 18 ? "Too young" : "Old enough"
alert(message)
// Connect js to html to see the result.

```

## Problem Sheet-2
### 1. Write a function to convert Celsius to Fahrenheit. The function should take a single argument, which is the temperature in Celsius.
##### Solution(js) :
```javascript
function celsiusToFahrenheit(celsius) {
    return (9 * celsius)/ 5 + 32;
}

console.log(celsiusToFahrenheit(0)); // 32
console.log(celsiusToFahrenheit(25)); // 77

```
### 2.  Write a function to check if a number is even. The function should take a single argument, which is the number to check.
##### Solution(js) :
```javascript
function isEven(num) {
  return num % 2 == 0;
}

console.log(isEven(4)); // true
console.log(isEven(7)); // false
```
### 3. Write a function to sum two numbers. The function should take two arguments, which are the numbers to sum.
##### Solution(js) :
```javascript
function sum(a, b) {
  return a + b;
}

console.log(sum(3, 4)); // 7
console.log(sum(10, 20)); // 30


```
### 4. Write a function to find the smallest number in an array. The function should take a single argument, which is the array to search.
##### Solution(js) :
```javascript
function findSmallestNum(arr) {
  return Math.min(...arr);
}

console.log(findSmallestNum([3, 5, 1, 9])); // 1
console.log(findSmallestNum([-1, -5, 0, 10])); // -5



```
### 5. Write a function to count the number of vowels in a string. The function should take a single argument, which is the string to search
##### Solution(js) :
```javascript
function countVowels(str) {
  let vowels = 'aeiouAEIOU';
  let count = 0;
for (let i = 0; i < str.length; i++) {
        if (vowels.includes(str[i])) {
            count++;
        }
    }
    
  return count;
}

console.log(countVowels("hello world")); // 3
console.log(countVowels("Javascript")); // 3


```
### 6.  Write a function to get the first element of an array. The function should take a single argument, which is the array.
##### Solution(js) :
```javascript
function getFirstElement(arr) {
      return arr.length > 0 ? arr[0] : undefined;

}

console.log(getFirstElement([1, 2, 3])); // 1
console.log(getFirstElement(["a", "b", "c"])); // "a"


```
###  7. Write a function to check if an array is empty. The function should take a single argument, which is the array.
##### Solution(js) :
```javascript
function isArrayEmpty(arr) {
      return arr.length > 0 ? "false" : "true"

}

console.log(isArrayEmpty([])); // true
console.log(isArrayEmpty([1, 2, 3])); // false


```
### 8. Write a function to return the factorial of a number. The function should take a single argument, which is the number.
##### Solution(js) :
```javascript


function factorial(num) {
    if (num === 0 || num === 1) return 1;
    if(num < 0 )  return  "Factorial is not defined for negative numbers";
    if(num > 1){
        let result = 1;
        for (let i = 1; i <=num; i++) {
            result *= i;
        }
        return result;
        
        
    }
  }
  
  console.log(factorial(5)); // 120
  console.log(factorial(7)); // 5040
  

```
### 9. Write a function to reverse a string. The function should take a single argument, which is the string to reverse.
##### Solution(js) :
```javascript
function reverseString(str) {
      return str.split('').reverse().join('');

}

console.log(reverseString("hello")); // "olleh"
console.log(reverseString("world")); // "dlrow"


```
### 10. Write a function to convert a string to lowercase. The function should take a single argument, which is the string to convert.
##### Solution(js) :
```javascript

function toLowerCase(str) {
      return str.toLowerCase();

}

console.log(toLowerCase("HELLO WORLD")); // "hello world"
console.log(toLowerCase("JavaScript")); // "javascript"

```
### 11. Write a function to find the length of a string. The function should take a single argument, which is the string.
##### Solution(js) :
```javascript
function stringLength(str) {
      return str.length;

}

console.log(stringLength("hello")); // 5
console.log(stringLength("world")); // 5


```
### 12.  Write a function to merge two arrays. The function should take two arguments, which are the arrays to merge.
##### Solution(js) :
```javascript
function mergeArrays(arr1, arr2) {
      return arr1.concat(arr2);

}

console.log(mergeArrays([1, 2, 3], [4, 5, 6])); // [1, 2, 3, 4, 5, 6]
console.log(mergeArrays(["a", "b"], ["c", "d"])); // ["a", "b", "c", "d"]


```
### 13.  Write a function to get the last element of an array. The function should take a single argument, which is the array.
##### Solution(js) :
```javascript
function getLastElement(arr) {
      return arr[arr.length-1];

}

console.log(getLastElement([1, 2, 3])); // 3
console.log(getLastElement(["a", "b", "c"])); // "c"


```

### 14.  Write a function to get the first character of a string. The function should take a single argument, which is the string.
##### Solution(js) :
```javascript
function getFirstCharacter(str) {
      return str.charAt(0);

}

console.log(getFirstCharacter("hello")); // "h"
console.log(getFirstCharacter("world")); // "w"


```
### 15.  Write a function to find the sum of all elements in an array. The function should take a single argument, which is the array. 
##### Solution(js):
```javascript
function sumArray(arr) {
  let sum = 0;
    for (let i = 0; i < arr.length; i++) {
      sum += arr[i];
    }
  return sum;
}

console.log(sumArray([1, 2, 3, 4])); // 10
console.log(sumArray([-1, -2, -3, -4])); // -10
console.log(sumArray([1.5, 2.5, 3.5])); // 7.5


```
# The other problem sheet is README.md




 

