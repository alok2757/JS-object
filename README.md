## JS-object

## Object -

object is an unordered collection of key-value pairs. Each key-value pair is called a property.<br>
The key of a property can be a string. And the value of a property can be any value, e.g., a string, a number, an array, and even a function.<br>
JavaScript provides  many ways to create an object. most commonly used one is to use the object literal notation.

##  https://www.javascripttutorial.net/javascript-objects

## Creating a JavaScript Object -

## 1.using an object literal.<br>
const person = {firstName:"John", lastName:"Doe", age:50, eyeColor:"blue"};

## 2.Create object with the keyword new.<br>
const person = new Object();
person.firstName = "John";
person.lastName = "Doe";
person.age = 50;
person.eyeColor = "blue";

## 3.Define an object constructor, and then create objects of the constructed type.<br>
## 4.Create an object using Object.create().


## Note-1.For readability, simplicity and execution speed, use the object literal method.
## 2. JavaScript Objects are Mutable.
Objects are mutable: They are addressed by reference, not by value.

## Nested Objects-
myObj = {
  name:"John",
  age:30,
  cars: {
    car1:"Ford",
    car2:"BMW",
    car3:"Fiat"
  }
}
console.log(myObj.cars.car2);
myObj.cars["car2"];

## We can access nested objects using the dot notation or the bracket notation.

## Object Accessors-
Getters and setters allow you to define Object Accessors.

![image](https://user-images.githubusercontent.com/122484692/211986147-c006b941-9e2e-42f8-a500-dcea9eb3f698.png)

![image](https://user-images.githubusercontent.com/122484692/211986202-ef540c77-0d94-4ace-b65a-7a9a76c9307d.png)

# JavaScript Object Constructors-
## Constructor function for Person objects-
function Person(first, last, age, eye) {
  this.firstName = first;
  this.lastName = last;
  this.age = age;
  this.eyeColor = eye;
}

## Create a Person object-
const myFather = new Person("John", "Doe", 50, "blue");


