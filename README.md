# kotlin-cheatsheet

### 1. Hello World

```kotlin
fun main() {
  println("Hello World!")
```

### 2. var vs val
`var` is used to declare a mutable variable i.e value **can** be changed.

`val` is used to declare an immutable variable i.e value **can't** be changed.

```kotlin
var name: String = "Sam" // mutable
name = "Abhishek"

val anotherName: String = "Sam" // immutable
anotherName = "Abhishek" // compilation error
```
