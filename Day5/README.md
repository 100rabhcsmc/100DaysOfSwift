<div align='center'>
    <h1>Day 5</h1> 
    <a class="header-badge" target="_blank" href="https://www.linkedin.com/in/saurabhmchavan/">
          <img src="https://img.shields.io/badge/style--5eba00.svg?label=LinkedIn&logo=linkedin&style=social">
    </a>   
    <a class="header-badge" target="_blank" href="https://twitter.com/100rabhcsmc">
          <img src="https://img.shields.io/badge/style--5eba00.svg?label=twitter&logo=twitter&style=social">
    </a>
 </div>

<div align='center'>
    <h1> Functions</h1> 
</div>

Functions let us re-use code, which means we can write a function to do something interesting then run that function from lots of places.
Repeating code is generally a bad idea, and functions help us avoid doing that.

```
func printHelp() {
    let message = "Namste Swift"

    print(message)
}
```

Run using

```
printHelp()
//output: Namste Swift

```

## 1.Accepting parameter

Values sent into functions this way are called parameters.

```
func sauChavan(Parameter: DataType){
//code
}

sauChavan(Parameter: argument)
```

```
func sauChavan(Surname:String){
let name="saurabh \(Surname)"
print(name)
}

sauChavan(Surname:"Chavan")
//Output: saurabh chavan

```

## 2.Returning values

```

func square(number: Int) -> Int {
return number \* number
}

let result = square(number: 8)
print(result)

```

## 3.Parameter labels

```

func sayHello(to name: String) {
print("Hello, \(name)!")
}

sayHello(to: "Saurabh")
//output: Hello Saurabh

```

## 4.Omitting parameter labels

```
//when we are not pass parameter

func Hello(_ person: String) {
print("Hello, \(person)!")
}
Hello("Saurabh")
//output: Hello Saurabh

```

You can refer here also best Way and easy <a  href="https://www.programiz.com/swift-programming/functions">Function </a>
