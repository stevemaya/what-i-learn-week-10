# Monday
## console.clear()
A function that clean up what displaced in the terminal. Like an eraser or refresh.

## readline function:
* A function that take in as a string and a function as a paramenter. Print out the string, wait for user input, store in a parameter, and then run the given function
* readline can be use with different method, like **readline.prompt**, **readline.question**, **readline.answer**, etc... (like string and array has its own methods)

~~~
// require 2 lines below to use readline function. 'readline' is a seperate file of code
const readline = require('readline')
const interface = readline.creatInterface({input: process.stdin, output: process.stout})

// pesuodo code of a readline function
function readline.question(string, function) {
console.log(string)
// wait for userinput. store it in a variable ('answer')
function() //run function
}

// Example:
readline.question('how many minutes in an hour?', sixtyMins())

sixtyMins(){
console.log(`There're 60 minutes in an hour`)
} 
~~~

# Tuesday
## object
syntax
~~~
const object = {
name: 'Huong'.  //-> name: property / key, 'Huong' is the value of that property / key
age: 300
alive: true
other: ['asian', 'female']
}
~~~
## object properties:
~~~
//1 add new property
object.address = 'Manhattan'
object['add address'] = 'Midtown, Manhattan' //use this way when keyname has space or is a number

//2 change value of a property
object.address = 'New jersey'
Object.defineProperty(object, address, {value : "overwritten DYNAMICALLY"}) // this way to use in a function

//3 push value into an array inside an object
object.other.push('brown eye', 'black hair', 'short')

//4 Check if there is a specific key in an object:
let check1 = 'age' in object //-> check1 = true/ false
let check2 = object.name === undefined  //-> check2. = true/false

//5 Change key name 'firstName' to 'lastName' in an object:

let person3 = { firstName: 'IDK', age: 1000, }
person3.lastName = person3.firstName
delete person3.firstName
person3; // -> { lastName: 'IDK', age: 1000, } 

//6 Can set a default value for paramenter when use a function for object
const makeDino = function (newName, newTime, newDiet, newExtinct = false) { //-> extinct default tobe false
    return {
      species: newName,
      period: newTime,
      carnivore: newDiet,
      extinct: newExtinct
    }
}
~~~
# Thursday
## Slice()
’String’.slice(a,b)
a: include in the new string
b: does not included in new string


let cutText = 'hello'.slice(0, str.length-2) // equal  'hello'.slice(0, -2)
cutText;
