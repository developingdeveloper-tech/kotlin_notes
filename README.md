# Kotlin Cheatsheet

## <a name="table-of-contents"></a>Table of Contents
  - [Hello World](#hello-world)
  - [var vs val](#var-vs-val)
  - [Data Types](#data-types)
  - [Null Safety](#null-safety)
  - [Different types of function declarations](#different-types-of-function-declarations)

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

### <a name="different-types-of-function-declarations"></a> Different types of function declarations <sup>[Back ⇈](#table-of-contents)</sup>
There are multiple ways to declare functions in kotlin.

```kotlin
fun main() {
    val num1 = 10
    val num2 = 20
    
    val sum        = add(num1, num2) // 30
    val difference = subtract(num1, num2) // -10
    val product    = multiply(num1, num2) // 200
    val quotient   = num2.divide(num1) // 2
    val remainder  = num2 % num1 // 0
}

fun add(num1: Int, num2: Int): Int { return num1 + num2 } // regular function

fun subtract(num1: Int, num2: Int): Int = num1 - num2 // like an expression
 
fun multiply(num1: Int, num2: Int) = num1 * num2 // return type is inferred

fun Int.divide(num2: Int) = this / num2 // extension function
```
