# Kotlin Cheatsheet

## <a name="table-of-contents"></a>Table of Contents
  - [Hello World](#hello-world)
  - [var vs val](#var-vs-val)

### <a name="hello-world"></a>Hello World <sup>[Back ⇈](#table-of-contents)</sup>

```kotlin
fun main() {
  println("Hello World!")
```

### <a name="var-vs-val"> var vs val <sup>[Back ⇈](#table-of-contents)</sup>
`var` is used to declare a mutable variable i.e value **can** be changed.

`val` is used to declare an immutable variable i.e value **can't** be changed.

```kotlin
var name: String = "Sam" // mutable
name = "Abhishek"

val anotherName: String = "Sam" // immutable
anotherName = "Abhishek" // compilation error
```
