<div align='center'>
    <h1>Day 9</h1> 
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
    <h1> Structs Part 9</h1> 
</div>

## Day 9

## Structs Part 2

**Initializers**

Initializers are special methods that provide different ways to create your struct. All structs come with one by default, called their memberwise initializer

```

struct User {
    var username: String
}

var user = User(username: "Saurabh")

print(user.username) //Saurabh
```

We can provide our own initializer to replace the default one. For example, we might want to create all new users as “Anonymous” and print a message, like this:

```
struct User {
    var username: String

    init() {
        username = "Anonymous"
        print("Creating a new user!")
    }
}
```

our initializer accepts no parameters, we need to create the struct like this:

```
var user = User()
user.username = "Saurabh"

print(user.username)
//Saurab
```
