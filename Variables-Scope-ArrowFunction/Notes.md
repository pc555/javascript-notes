### var vs let/const

- var variable is function scope and let/const is block scope
- let variable can not be redeclare in the same scope (var can, that can cause bugs)
- const you can not reassign value. However, if const variable is an object, you can change properties of the object
- some people use function(){} to wrap around javascript code is to avoid leaking to global scope

#### Temporal Dead Zone
- Accessing a var before it is declared has the result undefined; accessing a let or const before it is declared throws ReferenceError


### Arrow function

- Arrow function is always an anonymous function
- if no bracket{} after arrow function, it implicit return that statement, no need return keyword 
- if wants to implicit return object, put () arount that object{}
- be careful using arrow function with this keyword!! 

### Default Arguments

- You can set default arguments in the function to certain value
- If you want to pass new value into the function with default arguments and does not want to change some of the default value, simply pass undifined to the function
