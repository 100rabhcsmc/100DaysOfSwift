<div align='center'>
    <h1>Day 10</h1> 
    <a class="header-badge" target="_blank" href="https://www.linkedin.com/in/saurabhmchavan/">
          <img src="https://img.shields.io/badge/style--5eba00.svg?label=LinkedIn&logo=linkedin&style=social">
    </a>   
    <a class="header-badge" target="_blank" href="https://twitter.com/100rabhcsmc">
          <img src="https://img.shields.io/badge/style--5eba00.svg?label=twitter&logo=twitter&style=social">
    </a>
    <a class="header-badge" target="_blank" href="https://instagram.com/100rabhch">
          <img src="https://img.shields.io/badge/style--5eba00.svg?label=instagram&logo=instagram&style=social">
    </a>
    <a class="header-badge" target="_blank" href="https://stackoverflow.com/users/12053852/saurabh-chavan?tab=profile">
          <img src="https://img.shields.io/badge/style--5eba00.svg?label=stackoverflow&logo=stackoverflow&style=social">
    </a>
 </div>

<div align='center'>
    <h1>Classes and inheritance</h1> 
</div>

## Day 10

## Classes and inheritance

Similar to constants, variables and functions the user can define class properties and methods

Classes are similar to structs in that they allow you to create new types with properties and methods, but they have five important differences

**Creating your own classes**

The first difference between classes and structs is that classes never come with a memberwise initializer. This means if you have properties in your class, you must always create your own initializer.

```
class FullName {
    var firstName: String
    var lastName: String

    init(firstName: String, lastName: String) {
        self.firstName = firstName
        self.lastName = lastName
    }
}

let FName = FullName(firstName: "Saurabh", lastName: "Chavan")
print(FName.firstName)
//Saurabh
```

**Class inheritance**

Inheritance allows us to create a new class from an existing class.

The new class that is created is known as subclass (child or derived class) and the existing class from which the child class is derived is known as superclass (parent or base class).

we use the colon : to inherit a class from another class.

**Syntax:**

```
// define a superclass
class Animal {
  // properties and methods definition
}

// inheritance
class Dog: Animal {

  // properties and methods of Animal
  // properties and methods of Dog
}
```

Here, we are inheriting the Dog subclass from the Animal superclass.

**Example:**

```
class Animal {

  // properties and method of the parent class
  var name: String = ""

  func eat() {
    print("I can eat")
  }
}

// inherit from Animal
class Dog: Animal {

  // new method in subclass
  func display() {

    // access name property of superclass
    print("My name is ", name);
  }
}

// create an object of the subclass
var labrador = Dog()

// access superclass property and method
labrador.name = "Rohu"
labrador.eat()

// call subclass method
labrador.display()

**Output**

I can eat
My name is Rohu
```

**Example 2:**

```
class Sau {
    var name:String = ""
}

class Saurabh:Sau {
    func display(){
        print("My name is",name)
    }
}

let FName = Saurabh()
FName.name = "Saurabh"
FName.display()
//output
My name is Saurabh
```

**Overriding methods**

Child classes can replace parent methods with their own implementations – a process known as overriding.

if the same method is defined in both the superclass and the subclass, then the method of the subclass class overrides the method of the superclass. This is known as overriding.

**Syntax:**

```
class Vehicle {

  func displayInfo(){
    ...
  }
}

class Car: Vehicle {

  // override method
  override func displayInfo() {
    ...
  }
}
```

**Final classes**

Swift gives us a final keyword just for this purpose: when you declare a class as being final, no other class can inherit from it. This means they can’t override your methods in order to change your behavior – they need to use your class the way it was written.

To make a class final just put the final keyword before it

```
final class FullName {
    var Fname: String
    var Lname: String

    init(Fname: String,var Lname: String: String) {
        self.Fname = Fname
        self.Lname = Lname
    }
}
```
