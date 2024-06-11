# Javascript quiz (Basic Level 4)

1. What are anonymous functions in JavaScript?<br>
Ans. An anonymous function is the function that has no name,there is no identification when it is created.<br>

2. Explain strict comparison and Abstract comparison in javascript?<br>
Ans. strict comparision compares the value as well as the type of variable whereas abstract comparision compares only the value of variables.<br>

3. Difference b/w arrow functions and regular functions?<br>
Ans. Arrow functions do not have thier own "this" context,they capture the "this" value from the lexical context where arrow function is created on the other hand regular functions have their own "this" context.<br>

4. What is Hoisting in JavaScript?<br>
Ans. Hoisting in javascript refers to the built-in behaviour of the language through which declarations of classes,variables and functions are moved to the top of their scope-all before code execution.In return this allows us to use functions,variables and classes before declaration.<br>

5. JavaScript is a garbage collected programming language, explain how?<br>
Ans. Javascript automatically free up memory that is no longer being used that's why it is called garbage collected language.<br>

6. Explain Shallow copy vs Deep copy in Javascript?<br>
Ans. Shallow copy and Deep copy in Javascript are two ways to copy objects.shallow copy creates a new object with references to the same memory locations as the original object, while deep copying creates a new object with new memory locations for all of its properties.<br>

7. What is Object.freeze?
Ans. The object.freeze() method is used to freeze an object.Freezing an object does not allow new properties to be added to the object and prevents removing or altering the existing properties.object.freeze() preserves the enumerability, writability, configurability and prototype of the object.<br>

we can understand object.freeze with code:

```javascript

const obj = {
  lastname: 'mishra',
  age:22
}

Object.freeze(obj)

obj.lastname = 'vishwas'

console.log(obj)
```



1. Write a function that generates a random number between two ranges, -100 to 0 and 800 - 900.

```Javascript

function randomnumber(){

  function randint(min,max){
    return Math.floor(Math.random() * (max - min + 1) + min)
  }

  const pickednum = Math.random();

  if(pickednum < 0.5){
    return randint(-100,0)
  }
  else{
    return randint(800,900)
  }
}

console.log(randomnumber())

```

