# Javascript quiz (Basic Level - 3)

1. Explain as much as you know about objects in javascript? (A long answer expected).
Ans. objects are reference data type in javascript.object is a collection of properties that are "key:value" pairs,these pairs are of same or different data types.keys must be of string datatype and values can hold item of any datatype.function behave like an object in javascript.we can access keys and values by writing "object.keys(object name)" and "object.values(object name").when the value of property is a function then it is known as method.

2. Read the code :
// This is an object based vector template
var vector = {
_x: 0,
_y: 0,
create: function(x,y){
var obj = Object.create(this);
obj.setX(x);
obj.setY(y);
return obj;
},
}
Can you make a “class” based alternative to it? Using Javascript OOP features.

```javascript
class vector{

    _x = 0;
    _y = 0;

    constructor(x,y){
        this._x = x;
        this._y = y;
    }
}
```

3. Do you think javascript is the language of the future?
Ans. yes,javascript is the language of future because it is widely used in web development,video games,apps and high in demand.js is essential for web developers nowadays.we can develop front-end or back-end both with the help of js frameworks.

``` Javascript

//1. Write code implementations of arr methods -

//a. forEach
//b. map
//c. filter
//d. reduce
//e. includes
//f. some
//g. every



const arr = [4,7,9,34,11,23,67,78,87,"world"]


//a. forEach
arr.forEach(element => {
    console.log(element);
})


//b. map
arr.map(element => {
    console.log(element * 2)
})

//c. filter
var major = arr.filter((value) => {
    return(value > 18);
})

console.log(major)

//d. reduce
var sum = arr.reduce((prev,next) => {
    return(prev + next);
},1)

console.log(sum)

//e. includes
console.log(arr.includes("world"))

//f. some
var check = arr.some(value => {
    return(value > 18)
})
console.log(check)

//g. every
var check = arr.every(value => {
    return(value > 18)
})
console.log(check)