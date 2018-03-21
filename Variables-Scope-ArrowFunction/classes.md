### ES6 classes

## Class, Function and Property Declaration
```javascript
class Person {
  // use constructor keyword to initialize values
  constructor(name, age) { 
    this.name = name;
    this.age = age;
  }
  
  // declaring a function (same as previous prototype function)
  move() {
    console.log(`${this.name} is walking`);
  }
  
  eat() {
    console.log('eating!');
  }
  
  //declaring static function (this funtion is bind to Person class)
  //to use this, call Person.info()
  static info() {
    console.log('A person has a name');
  }
  
  //set properties
  set nickname(value) {
    this.nick = value;
  }
  
  //get properties
  get nickname() {
    return this.nick;
  }
}
```
## Inheritance using extends
```javascript
class Baby extends Person {
  constructor(name) {
    super(name, 1); //use super keyword to call Person's constructor
  }
  
  //override parent class's function
  move() {
    console.log(`${this.name} is crawling`);
  }
  
  //Baby still has eat() function since it inherit Person's function
}
```
