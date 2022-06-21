# Day 1

## Variables,Data Type,String interpolation,Type annotations

1. You make variable using var and constant using let.

```
var mark = 45
let highestMark = 100
```

We can chnage variable using..

```
 mark = 45
 highestMark = 100
```

We don't need var and let second time its already been created.

2. String start and end with double quotes.

```
 var name = “saurabh”
```

3. For the multiple line of string you should use three sets of double quotes.

```
 var fullName = “““
                   saurabh
                   chavan
                 ”””
```

4. Integers hold whole number.

```
1, 2, -200
```

5. If you have large numbers, Swift lets you use underscores as thousands separators.

```
var population = 8_000_000
```

6.Double hold fractional number.

```
var Price = 10.2
```

7. Booleans hold true or false

```
 var job = true
```

8. You can place any type of variable inside your string.all you have to do is write a backslask\ followed by your varibale name in parantheses

```
var score = 87
     var str = “Your score was \(score)”
```

9.Constant:
I already said that variables have that name because their values can change over time, and that is often useful. However, very often you want to set a value once and never change it, and so we have an alternative to the var keyword called let.

The let keyword creates constants, which are values that can be set once and never again. For example:

```
let taylor = "swift"
```

If you try to change that, Xcode will refuse to run your code

10. Swift uses type interface to assign each variable or constant a type.
    Type annotations begin with a colon(:) and end with a type.

```
var name : String = “saurabh”
```
