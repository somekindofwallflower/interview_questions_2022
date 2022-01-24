
# JavaScript questions

### Basic

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
