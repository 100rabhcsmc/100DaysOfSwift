<div align='center'>
    <h1>Day 3</h1> 
    <a class="header-badge" target="_blank" href="https://www.linkedin.com/in/saurabhmchavan/">
          <img src="https://img.shields.io/badge/style--5eba00.svg?label=LinkedIn&logo=linkedin&style=social">
    </a>   
    <a class="header-badge" target="_blank" href="https://twitter.com/100rabhcsmc">
          <img src="https://img.shields.io/badge/style--5eba00.svg?label=twitter&logo=twitter&style=social">
    </a>
 </div>

<div align='center'>
    <h1>Operators and conditions</h1> 
</div>

Operators are special symbols that perform operations on variables and values.

**1.Arithmetic Operators**
Arithmetic operators are used to perform mathematical operations like addition, subtraction, multiplication.

```
let firstScore = 12
let secondScore = 4
```

Add And Subtract

```
let total = firstScore + secondScore
let difference = firstScore - secondScore
```

multiply and divided

```
let product = firstScore * secondScore
let divided = firstScore / secondScore
```

**2.Compound assignment operator**

```
var score = 95
score -= 5  //90
```

**3.Comparison Operator**
Comparison operators compare two values/variables and return a boolean result: true or false. For example,

```
var a = 5, b =2
print (a > b)      // true
```

```

Operator	Meaning 	Example
==	   Is Equal To 	        3 == 5 gives us false
!=	   Not Equal To 	3 != 5 gives us true
>	   Greater Than	        3 > 5 gives us false
<	   Less Than	        3 < 5 gives us true
>=	Greater Than or Equal To	3 >= 5 give us false
<=	Less Than or Equal To	        3 <= 5 gives us true
```

**4.Logical Operators**
Logical operators are used to check whether an expression is true or false. They are used in decision-making. For example,

```
var a = 5, b = 6
print((a > 2) && (b >= 6))    // true
```

```
Operator Example	  Meaning
&&       a && b	   Logical AND:true only if both the operands are true

||	a || b	   Logical OR:true if at least one of the operands is true
!	  !a	   Logical NOT:
true if the operand is false and vice-versa.

```

**Condition**
Example if else

```
let firstCard = 11
let secondCard = 10

if firstCard + secondCard == 21 {
    print("Blackjack!")
} else {
    print("Regular cards")
}

```

1. combining condition
   Swift has two special operators that let us combine conditions together: they are && (pronounced “and”) and || (pronounced “or”).

Example

```
let age1 = 12
let age2 = 21

if age1 > 18 && age2 > 18 {
    print("Both are over 18")
}

if age1 > 18 || age2 > 18 {
    print("At least one is over 18")
}
```

**The ternary operator**
Example

```
let firstCard = 11
let secondCard = 10
print(firstCard == secondCard ? "Cards are the same" : "Cards are different")
```

**Switch statements**

```
let weather = "sunny"

switch weather {
case "rain":
    print("Bring an umbrella")
case "snow":
    print("Wrap up warm")
case "sunny":
    print("Wear sunscreen")
default:
    print("Enjoy your day!")
}
```

**Range operators**
Swift includes two range operators, which are shortcuts for expressing a range of values. The following table explains these two operators.
1.Closed Range
(a...b) defines a range that runs from a to b, and includes the values a and b.
Example:

```
1...5 gives 1, 2, 3, 4 and 5
```

2.Half-Open Range

```
1..< 5 gives 1, 2, 3, and 4
```

<div align="right">
    <a href="https://github.com/100rabhcsmc/100DaysOfSwift/tree/main/Day4">
          Day 4 >>
    </a>
 </div>
