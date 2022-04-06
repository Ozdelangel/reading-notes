# Brush Up on ES6 syntax

## Legend
X - Variable
Obj - object
arr - Array
func - Function
a,b,c - parameter method
str - String


Scopes for different variable types

var - Function scope and can be reassigned and redeclared
let - block scope is no hoisting can be reassigned but not redeclared
const - cannot be reassigned and cannot be redeclared

## Variable Declaration

`let x = 0`

`var x = 0`

## arrow functions 
the arrow function is just a shorter way to creat a function - remember function do not have their own `this` - do not have prototypes - cannot be used for constructors - should not be used for object methods

regular - function func(a,b,c) {
    expression
}

es6 - let func = (a) => {
    expression
}

## Template literals

`${data}`
`${this.name}`
`${this.time}`


## implicit returns

regular - function func(a,b,c) {

    return a + b + + c
} 

ES6 
let func = (a, b, c) => a + b +c 

curly brackets can be omitted

## key property shorthand

es6 - let obj = {
    a,
    b,
}

instead of - var obj = {
    a:a,
    b:b,

}

## Array iteration or looping

for(let i of arr) {
    console.log(i)
}

## components and props

components let you split the UI into independent, reusable pieces, and think about each peace in isolation.

### functions and class components
the simplest way to define a component is to write a Javascript function 

function Welcome(props) {
  return <h1>Hello, {props.name}</h1>;
}

the function above is a valid react component because it accepts single props argument with data and returns a react element

you can also define a component with es6 classes

class Welcome extends React.Component {
  render() {
    return <h1>Hello, {this.props.name}</h1>;
  }
}

## Rendering a Component 

const element = <div />;

const element = <Welcome name="Sara" />;

so the above is saying that were passing down the name sara as props so it can be used somewhere else