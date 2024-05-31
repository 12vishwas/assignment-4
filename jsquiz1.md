# Javascript quiz (Basic Level - 1) 


1. What is JavaScript?
Ans. Javascript is a high level, interpreted, dynamically typed  scripting language that is widely used in front end development nowadays.

2. What is the difference between b/w let and var?
Ans. 'let' is block scoped.let can be declared globally but its  access is  only inside the block in which it is declared.we can update the value of variable but  cannot re-declare the variable using let within the same block.

'var' can be declared and accessed globally.it can be updated and re-declared within the same scope.

3. Why do we prefer const over var?
Ans. const keyword makes the variable immutable means we cannot reassign the variable's value and the code with less variance makes code reliable and easier to read.

4. What is the use of javascript in web browsers?
Ans.Javascript is a text based programming language used both on the client side and server side that allows us to make webpages interactive.

5. What are Objects?
Ans. object is a primitive data type in javascript.An object is a collection of properties that has pair of "key" and "value".

6. What is an array and how is it different from an Object in Javascript?
Ans. An array is a collection of elements of different or same data type but object is a collection of properties that are (key:value) pairs.

7. What is a function?
Ans. A set of statements which performs a particular task.we can create a function using 'function' keyword.

8. How can we implement call by value and call by reference in Javascript?
Ans In call by value a copy of original variable is created and in call by reference we pass the reference of the actual parameter,no copy is created in  the memory. 

9. What are the primitive data types in Javascript?
Ans. There are five primitive data types in javascript number,string,boolean,null,undefined.primitive data types are simple and built-in data types.

10. What is DOM?
Ans. DOM is 'Document object model' that is a programming interface for web documents.we can change the document structure ,style and content with the help of DOM.

11. Why do we need DOM?
Ans. with the help of DOM we can easily access and manipulate tags,IDs,attributes,classes and other elements of html and css using commands and methods provided by the document object.
***

```Javascript

//1. Average of array nums in Javascript?

var nums = [12,32,43,14,55,64]

var sum = nums.reduce((prev,curr) => {
    return prev + curr;
}, 0)

var average = (sum/(nums.length))

console.log(average)

//2. how to swap two numbers by reference in javascript?

var a = 10;
var b = 20;

var temp = a;
a = b;
b = temp;

console.log(a,b)

//3. Print the fibonacci sequence?

var a = 0;
var b = 1;



for(var i=1; i<15; i++){
    console.log(a)
    var sum = a + b;

    a=b;
    b=sum;

}

//4. Sort an array by both ascending and descending order?

const array = [3,11,32,0,55,44,87,75]

const sorted = array.sort()

console.log(sorted)

console.log(sorted.reverse())

//5. Show a variable value in an HTML webpage using DOM?

<html>
<head></head>
<body>
<h1>The value of number is:
<script>
var number = 10;

document.write(number)
</script>
</h1>
</body>
</html>

```