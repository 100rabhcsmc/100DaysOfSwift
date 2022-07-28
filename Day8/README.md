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
    <h1> Structs Part 8</h1> 
</div>

## Day 8

## Structs Part 1

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
