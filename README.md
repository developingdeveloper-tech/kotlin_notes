# Kotlin Cheatsheet

## <a name="table-of-contents"></a>Table of Contents
  - [Hello World](#hello-world)
  - [var vs val](#var-vs-val)
  - [Data Types](#data-types)
  - [Null Safety](#null-safety)

### <a name="hello-world"></a>Hello World <sup>[Back ⇈](#table-of-contents)</sup>

```kotlin
fun main() {
  println("Hello World!")
```

### <a name="var-vs-val"></a> var vs val <sup>[Back ⇈](#table-of-contents)</sup>
`var` is used to declare a mutable variable i.e value **can** be changed.

`val` is used to declare an immutable variable i.e value **can't** be changed.

```kotlin
var name: String = "Sam" // mutable
name = "Abhishek"

val anotherName: String = "Sam" // immutable
anotherName = "Abhishek" // compilation error
```
### <a name="data-types"></a> Data Types <sup>[Back ⇈](#table-of-contents)</sup>
  1. String
  2. Boolean
  3. Byte
  4. Short
  5. Int
  6. Long
  7. Float
  8. Double

```kotlin
val name: String = "Hello world!"
    
val isVerified: Boolean  = true // or false

val byte: Byte = 20
val one: Int = 1
val number: Long = 123456789

val floatNumber: Float = 123.52f
val pi: Double = 3.14
```

### <a name="null-safety"></a> Null Safety <sup>[Back ⇈](#table-of-contents)</sup>
Kotlin has a strong type system which means, variables can either hold null or they can't.

```kotlin
 var name: String = "John Doe"
name = null // invalid (error)

var nullableName: String? = "John Doe"
nullableName = null // valid

var age: Int = null // invalid (error)

var nullableAge: Int? = 10
nullableAge = null // valid

val students = mutableListOf<String>()
students.add(null) // invalid (error)

val nullableStudents = mutableListOf<String?>()
nullableStudents.add(null) // valid
```
