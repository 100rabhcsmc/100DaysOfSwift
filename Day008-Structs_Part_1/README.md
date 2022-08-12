<div align='center'>
    <h1>Day 8</h1> 
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
    <h1> Structs Part 1</h1> 
</div>

## Day 8

## Structs Part 1

**Creating your own structs**

In Swift, a struct is used to store variables of different data types.

structures, which are a “named type”. Like a String, Int or Array, you can define your own structures to create named types to later use in your code

Variables inside structs are called properties.

Structs can be given their own variables and constants, and their own functions, then created and used however you want.

```
struct Sport {
   var name: String
}
```

That defines the type, so now we can create and use an instance of it:

```
var tennis = Sport(name: "Tennis")
print(tennis.name)

Output:
Tennis

tennis.name = "Lawn tennis"
print(tennis.name)

Output:
Lawn tennis
```

Properties can have default values just like regular variables, and you can usually rely on Swift’s type inference.

**Computed properties**

```
struct Sport {
    var name: String
}
```

That has a name property that stores a String. These are called stored properties, because Swift has a different kind of property called a computed property – a property that runs code to figure out its value.

```
struct Sport {
    var name: String
    var isOlympicSport: Bool

    var olympicStatus: String {
        if isOlympicSport {
            return "\(name) is an Olympic sport"
        } else {
            return "\(name) is not an Olympic sport"
        }
    }
}

let chessBoxing = Sport(name: "Chessboxing", isOlympicSport: false)
print(chessBoxing.olympicStatus)

Output:
Chessboxing is not an Olympic sport
```

**Property observers**

```
struct Progressa {
    var task: String
    var amount: Int {
        didSet {
            print("\(task) is now \(amount)% complete")
        }
    }
}


var progress = Progressa(task: "Loading data", amount: 0)
progress.amount = 30
progress.amount = 80
progress.amount = 100

Output:
Loading data is now 30% complete
Loading data is now 80% complete
Loading data is now 100% complete
```

What we want to happen is for Swift to print a message every time amount changes, and we can use a **didSet** property observer for that. This will run some code every time amount changes:

You can also use **willSet** to take action before a property changes, but that is rarely used.

**Methods**

Structs can have functions inside them, and those functions can use the properties of the struct as they need to. Functions inside structs are called methods.

```
struct City {
    var population: Int

    func collectTaxes() -> Int {
        return population * 1000
    }
}

let london = City(population: 9_000_000)
london.collectTaxes()
```

**Mutating methods**

If a struct has a variable property but the instance of the struct was created as a constant, that property can’t be changed.

When you want to change a property inside a method, you need to mark it using the mutating keyword, like this:

```
struct Person {
    var name: String

    mutating func makeAnonymous() {
        name = "Anonymous"
    }
}

var person = Person(name: "Ed")
person.makeAnonymous()

print(person.name)

Output:
Anonymous
```

**Properties and methods of strings**

```
let string = "Welcome to 100Days Of Swift"

print(string.count)  //27
```

They have a hasPrefix() method that returns true if the string starts with specific letters:

```
print(string.hasPrefix("Sau")) //false

print(string.hasPrefix("Welcome")) //true

print(string.uppercased()) //WELCOME TO 100DAYS OF SWIFT

```

<div align="right">
    <a href="https://github.com/100rabhcsmc/100DaysOfSwift/tree/main/Day9">
          Day 9 >>
    </a>
 </div>
