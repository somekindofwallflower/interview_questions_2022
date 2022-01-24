
# Technical interview

### Break the ice

What will be the output of the following code?

1) 
```
function Add(){
    console.log(answer)
    var answer = 2
};
Add()
```
2)
```
var temp = "hi"
function display(){
  var temp
  console.log(temp)
  temp = "bye" 
}
display()
```

### Array Destructuring

What will be the output of the following code?

1)
``` 
function arrayDestructuring (list) {
  const [, , ...arr] = list; 
  return arr;
} 
var arrLiteral = [8,9,10,11,12]
console.log("arr contains: " + arrayDestructuring(arrLiteral))
```

2)

``` 
var arrLiteral = [8,9,10,11,12]
const [value1, value2] = arrLiteral
console.log("value1 is: " + value1)
console.log("value2 is: " + value2)
```

### Destructure undefined

```
function pointValues(point){
    const {name:n,age:a} = {...point} 
    console.log(n)
    console.log(a)
}
pointValues({name:"jerry", age:2})
pointValues(undefined)
```

### Type coercion
What will be the output of the code below?

```

var names = ["Tom","Anna",2,true]
console.log(names instanceof String)
console.log(names instanceof Number)
console.log(names instanceof Object)
console.log(names instanceof Array)

```

### Arrays
What will be the output of the code below?

```

function check(obj) {
  if (Object.prototype.toString.call(obj) === "[object Array]") {
    return true;
  } else {
    return false;
  }
}
console.log(check(123));
console.log(check("cat"));
console.log(check([1, 2, 3, 4]));

```

### Instance of array?
What will be the output of the code below?

1.
```
function check(){
    var tempFunc = function () {}
    console.log(typeof tempFunc)
    return new tempFunc instanceof Array; 
}
console.log(check())

```

2,
```
function check(){
    var tempFunc = function () {}
    tempFunc.prototype = Array.prototype
    return new tempFunc instanceof Array; 
}
console.log(check())
```

### Shallow copying

What will be the output of the code below?

```
const girl = {
  name: 'Anna',
  info: { age: 20, number: 123 }
};

const newGirl = { ...girl };
newGirl.info.age = 30;
console.log(girl.info.age, newGirl.info.age);
```

### Higher order functions

Is the function below a higher order function?
```
const func1 = function(num){
  return function(){
    if(typeof num == 'NaN'){
      return "Not a number"
    }else{
      return typeof(num)
    }
  }
}
```

### Data structures and algorithms

Result of the executing the function is?

```
function problem1(arr) {
    var odds = []
    for (let number of arr) {
        if (number % 2 != 0)
            odds.push(number)
    }
  return odds // Return the new list
}
console.log(problem1([3, 2, 41, 3, 34]))
```
