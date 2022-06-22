<div align='center'>
    <h1>Day 2</h1> 
    <a class="header-badge" target="_blank" href="https://www.linkedin.com/in/saurabhmchavan/">
          <img src="https://img.shields.io/badge/style--5eba00.svg?label=LinkedIn&logo=linkedin&style=social">
    </a>   
    <a class="header-badge" target="_blank" href="https://twitter.com/100rabhcsmc">
          <img src="https://img.shields.io/badge/style--5eba00.svg?label=twitter&logo=twitter&style=social">
    </a>
 </div>

<div align='center'>
    <h1>Arrays, sets, Tuples, dictionaries and enums</h1> 
</div>

1.Swift’s strings, integers, Booleans, and Doubles allow us to temporarily store single values, but if you want to store many values you will often use arrays instead.

**An array** stores values of the same type in an ordered list.

```
var Names: [String] = ["Saurabh","Sachin"]
```

Array position start with 0,so if you want to read sachin then

```
Name[1]
```

2. **Sets** are unordered collections of unique values.

```
var favoriteGenres: Set<String> = ["Rock", "Classical", "Hip hop"]

or

var favoriteGenres: Set = ["Rock", "Classical", "Hip hop"]


```

If you try to insert a duplicate item into a set, the duplicates get ignored.

```
var favoriteGenres: Set = ["Rock", "Classical", "Hip hop","Rock","Classical"]
```

You can create set from Array

```
var Names= set(["Saurabh","Sachin"])
```

3.**Tuples** are created by placing multiple items into parentheses, like this:

```
var name = (first: "Saurabh", last: "Chavan")

```

access item from tuple

```
name.0
or
name.first
```

Remember, you can change the values inside a tuple after you create it, but not the types of values. so if you tried to change name to be (first: "Justin", age: 25) you would get an error.

4.**A dictionary** stores associations between keys of the same type and values of the same type in a collection with no defined ordering

```
var someDict:[Int:String] = [1:"One", 2:"Two", 3:"Three"]
```

5.According to the Swift documentation enumeration is defined as “a common type for a group of related values and enables you to work with those values in a type-safe way within your code”.
for more details about enum [Click Here..](https://codewithchris.com/swift-enum/)

6.Creating empty collections
Arrays, sets, and dictionaries are called collections, because they collect values together in one place.
Empty Dictionary

```
var teams = [String: String]()
```

we can add

```
teams["Paul"] = "Red"
```

empty Array

```
var results = [Int]()
```

empty set

```
var words = Set<String>()
var numbers = Set<Int>()
```
