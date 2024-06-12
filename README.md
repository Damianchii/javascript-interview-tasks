
# 🚀 JavaScript Interview Tasks 
<p align="center">
  <a href="https://skillicons.dev">
    <img src="https://skillicons.dev/icons?i=js" />
  </a>
</p>

## ➡️ What will be returned by each of these?

```bash
console.log("hello" || "world")
console.log("foo" && "bar")

```
### Returned

```bash
Hello
bar


```

## ➡️ Write a JavaScript function to calculate the sum of two numbers. 

```bash
const sum = function(a,b) {
    return a + b
}

sum(1,2)
```
### Returned
```bash
3
```

## ➡️ Write a JavaScript program to find the maximum number in an array.

```bash
const arr = [1,2,3,4,5,6,7,10]

const maxNumber =  function(arr){
  let result = Math.max(...arr)
  return result

}
```
### Returned
```bash
10
```

## ➡️ Write a JavaScript function to check if a given string is a palindrome (reads the same forwards and backwards). 

> A palindrome means that a word means the same thing in reverse

```bash
const isPalindrome = (str) => {
  return str === str.split("").reverse().join("")

}

console.log(isPalindrome("kajak"))
```
### Returned

```bash
true
```

## ➡️ Write a JavaScript program to reverse a given string. 

```bash
const reverseString = (str) => {
  return str.split("").reverse().join("")
}

console.log(reverseString("hello"))
```

### Returned
```bash
olleh
```

## ➡️ Write a JavaScript function that takes an array of numbers and returns a new array with only the even numbers. 

```bash
const arr = [1,2,3,4,5,6,7,8,9,10]

const evenArr = arr => {
  return arr.filter((number) => number % 2 === 0)
}

console.log(evenArr(arr))

```

### Returned
```bash
2,4,6,8,10
```

## ➡️ Write a JavaScript program to calculate the factorial of a given number. 

> Thats how factorial looks like
> 5! = 5 * 4 * 3 * 2 * 1

```bash
function calculateFactorial(number) {
  if (number === 0 || number === 1) {
    return 1;
  } else {
    return number * calculateFactorial(number - 1);
  }
}

console.log(calculateFactorial(5))

```
### Returned

```bash
120
```

## ➡️ Write a JavaScript function to check if a given number is prime. 

```bash
function isPrime(number) {
  if (number <= 1) {
    return false;
  }
  if (number <= 3) {
    return true;
  }
  if (number % 2 === 0 || number % 3 === 0) {
    return false;
  }
  for (let i = 2; i <= Math.sqrt(number); i++) { 

    if (number % i === 0) return false; 

  } 
  return true;
}

console.log(isPrime(5))

```
### Returned

```bash
true
```

## ➡️ Write a JavaScript program to find the largest element in a nested array. 

```bash
const fibonacciSequence = function(num){
  const fibonacci = [0,1]
  
  if(num <= 0){
    return []
  }
  
  if(num === 1){
    return [0]
  }
  
    if(num === 2){
    return fibonacci
  }
  
  for(let i = 3; i <= num; i++){
    fibonacci.push(fibonacci[fibonacci.length-1] + fibonacci[fibonacci.length-2])
  }
  
  return fibonacci
}


console.log(fibonacciSequence(10))
```

### Returned

```bash
0,1,1,2,3,5,8,13,21,34,55
```

## ➡️ Write a JavaScript program to convert a string to title case (capitalize the first letter of each word). 

```bash
function toTitleCase(str) { 

  return str.replace(/\b\w/g, l => l.toUpperCase()); 

} 

console.log("hello world")
```

### Returned

```bash
Hello World

```
