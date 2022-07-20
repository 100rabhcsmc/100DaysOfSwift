<div align='center'>
    <h1>Day 6</h1> 
    <a class="header-badge" target="_blank" href="https://www.linkedin.com/in/saurabhmchavan/">
          <img src="https://img.shields.io/badge/style--5eba00.svg?label=LinkedIn&logo=linkedin&style=social">
    </a>   
    <a class="header-badge" target="_blank" href="https://twitter.com/100rabhcsmc">
          <img src="https://img.shields.io/badge/style--5eba00.svg?label=twitter&logo=twitter&style=social">
    </a>
    <a class="header-badge" target="_blank" href="https://instagram.com/100rabhch">
          <img src="https://img.shields.io/badge/style--5eba00.svg?label=instagram&logo=instagram&style=social">
    </a>
 </div>

<div align='center'>
    <h1> Closures Part 1</h1> 
</div>

## Day 6

## Closures Part 1

In Swift, a closure is a special type of function without the function name

Example

```
let Sau = {
    print("I'm Saurabh, iOS developer")
}

//call the Closure
Sau()
```

2.Closure with Parameter

We don't use the **func** keyword to create closure. Here's the syntax to declare a closure:

```
{ (parameters) -> returnType in
   // statements
}
Here,
```

**parameters** - any value passed to closure
**returnType** - specifies the type of value returned by the closure
**in (optional)** - used to separate parameters/returnType from closure body

Example

```
let Sau={ (name:String) in
print("MySelf \(name)")
}

//Call the Closure
Sau("Saurabh")
```

## return value in Closure

If we want our closure to return some value, we need to mention it's return type and use the return statement. For example,

```
/ closure definition
var findSquare = { (num: Int) -> (Int) in
  var square = num * num
  return square
}

// closure call
var result = findSquare(3)

print("Square:",result)
```

## Closure as parameter

closures can be used just like strings and integers, you can pass them into functions.

```
let driving = {
    print("I'm driving in my car")
}

func travel(action: () -> Void) {
    print("I'm getting ready to go.")
    action()
    print("I arrived!")
}

travel(action: driving)
```

If we wanted to pass that closure into a function so it can be run inside that function, we would specify the parameter type as () -> Void. That means “accepts no parameters, and returns Void” – Swift’s way of saying “nothing”.
