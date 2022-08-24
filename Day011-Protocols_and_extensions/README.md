<div align='center'>
    <h1>Day 11</h1> 
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
    <h1>Protocols and extensions</h1> 
</div>

## Day 11

## Protocols and extensions

**Protocols**

In Swift, a protocol defines a blueprint of methods or properties that can then be adopted by classes (or any other types).

We use the protocol keyword to define a protocol.
For example,

```
protocol Greet {

  // blueprint of a property
  var name: String { get }


  // blueprint of a method
  func message()
}
```

The protocol just holds the method or properties definition, not their actual body.

The protocol must specify whether the property will be gettable or gettable and settable.

**Protocol inheritance**

One protocol can inherit from another in a process known as protocol inheritance.

Unlike with classes, you can inherit from multiple protocols at the same time before you add your own customizations on top.

Example:

```
protocol Payable {
    func calculateWages() -> Int
}

protocol NeedsTraining {
    func study()
}

protocol HasVacation {
    func takeVacation(days: Int)
}
```

We can now create a single Employee protocol that brings them together in one protocol. We don’t need to add anything on top, so we’ll just write open and close braces:

```
protocol Employee: Payable, NeedsTraining, HasVacation { }
```

**Extensions**
