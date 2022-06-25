<div align='center'>
    <h1>Day 4</h1> 
    <a class="header-badge" target="_blank" href="https://www.linkedin.com/in/saurabhmchavan/">
          <img src="https://img.shields.io/badge/style--5eba00.svg?label=LinkedIn&logo=linkedin&style=social">
    </a>   
    <a class="header-badge" target="_blank" href="https://twitter.com/100rabhcsmc">
          <img src="https://img.shields.io/badge/style--5eba00.svg?label=twitter&logo=twitter&style=social">
    </a>
 </div>

<div align='center'>
    <h1> Loops</h1> 
</div>

the ability to repeat some simple task billions of times every second is called Loops.

\*\*For loop

```
let count = 1...10
for number in count {
    print("Number is \(number)")
}
```

Ans:

```
Number is 1
Number is 2
Number is 3
Number is 4
....
Number is 20
```

With underscore(\_)

```
for _ in 1...5 {
    print("Saurabh")
}
```

Ans:

```
Saurabh
Saurabh
Saurabh
Saurabh
Saurabh
```

**While Loop**
A second way of writing loops is using while: give it a condition to check, and its loop code will go around and around until the condition fails.

```
var number = 1

while number <= 10 {
    print(number)
    number += 1
}

```

Ans:

```
1
2
3
4
5
..
10
```

**Summary**
1.Loops let us repeat code until a condition is false.
2.If you don’t need the temporary constant that for loops give you, use an underscore instead so Swift can skip that work.
