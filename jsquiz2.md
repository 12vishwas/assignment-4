# Javascript quiz (Basic Level - 2)

1. Why do we use functions in JavaScript?
Ans. A function is a block of "reusable code" that is used several times in the program.it decreases the complexity of code by enabling re-usability.

2. What is Function Invocation?
Ans. Function Invocation is the process of calling a function.we can call it by writing function's name followed by a pair of parentheses.

3. Does a function behave like an object in Javascript? Prove it by an example.
Ans. Yes,function behave like an object in Javascript.we can understand with below example:

example:

```Javascript
const myobj = {
    myfunction : function(){
        console.log("my name is vishwas")
    }
}

myobj.myfunction()
```
In above example "myobj.myfunction()" is a function stored as an property  of an object.it demonstrates that the function behave like an object in javascript.


4. What are Events in Javascript?
Ans. An event is an action that occurs as per user's instruction and gives output in response.

5. What is a string?
Ans. A string is a sequence of characters that is used to represent text. string can be  written between double quotes.

6. What is an array? Is it static or dynamic in Javascript?
Ans. An array is a collection of items of same or different data types stored at contiguous memory locations. Javascript arrays are dynamic.

7. Difference between Map and Set?
Ans. Map is a collection of "key-value" pairs where keys can be of any datatype.map remembers its order of insertion and set is a collection of unique values.

8. Difference between Array and Map?
Ans. Array is a collection of items of same or different data types and map is a collection of "key-value" pairs where keys can be of any datatype.

9. What are array methods? List a few names?
Ans. Array methods are the built-in functions that are used to perform various operations on arrays like sorting,reduce,reverse.

10. In how many ways can we traverse through an array in Javascript?
As. We can traverse through an array in Javascript in following ways:
* Using console.log() Method
* Using for Loop
* Using while loop
* Using forEach() Method
* Using every() Method
* Using map() Method
* Using filter() Method
* Using reduce() Method
* Using some() Method
* Using entries() Method



 
```Javascript

//1. Reverse an array? Input: [1, 2, 3, 4, 5, 6]

const array = [1,2,3,4,5,6]

console.log(array.reverse())


//2. Explain the properties of the join array method function via program?

const items = [1, 2, 3, 4, 5, 6,"mango"]

console.log(items.join())

//join array method return string from array by concatenating array items separated by comma or specified seperator 

//3. Show all the values of an array in a html webpage using DOM and forEach method?


<html>
    <head>
        <title>Test</title>
    </head>
    <body>
        <p>Names of elements of array are: </p>
    </body>
        <script>
            const fruits = ["orange", "papaya", "pineapple", "mango"]

            fruits.forEach(value => {
                document.write(value + " ")
            })
        </script>
</html>

//4. Merge two sets in javascript? (hint use Set class in javascript)

var set1 = new Set([1,2,3])
var set2 = new Set([4,5,6])



const mergeset = new Set([...set1,...set2])

console.log(mergeset)

```