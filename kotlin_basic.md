
# 📘 Kotlin Basics Cheat Sheet

Kotlin is a statically typed programming language developed by JetBrains that runs on the JVM and can be used for Android development, server-side, or multiplatform development.

---

## ✅ 1. Hello World

```kotlin
fun main() {
    println("Hello, Kotlin!")
}
````

---

## 🟡 2. Variables

### Immutable (`val`) and Mutable (`var`):

```kotlin
val name = "John"        // read-only
var age = 25             // mutable
```

You don’t need to specify type; Kotlin has type inference. But you can if you want:

```kotlin
val city: String = "Paris"
var score: Int = 100
```

---

## 🔤 3. Data Types

| Type      | Example        |
| --------- | -------------- |
| `Int`     | `val num = 10` |
| `Long`    | `val l = 100L` |
| `Double`  | `val d = 3.14` |
| `Float`   | `val f = 2.5F` |
| `Boolean` | `val b = true` |
| `Char`    | `val c = 'A'`  |
| `String`  | `val s = "Hi"` |

---

## 🔁 4. Control Flow

### If-Else Expression:

```kotlin
val max = if (a > b) a else b
```

### When Expression (like switch):

```kotlin
val x = 3
val result = when (x) {
    1 -> "One"
    2 -> "Two"
    in 3..5 -> "Three to Five"
    else -> "Unknown"
}
```

---

## 🔂 5. Loops

### For Loop:

```kotlin
for (i in 1..5) {
    println(i)
}
```

### While Loop:

```kotlin
var i = 0
while (i < 5) {
    println(i)
    i++
}
```

### Do-While Loop:

```kotlin
var j = 0
do {
    println(j)
    j++
} while (j < 5)
```

---

## 🧮 6. Functions

```kotlin
fun add(a: Int, b: Int): Int {
    return a + b
}
```

### Single Expression Function:

```kotlin
fun square(x: Int) = x * x
```

---

## 📦 7. Null Safety

```kotlin
var name: String? = null  // nullable type
println(name?.length)     // safe call
println(name?.length ?: 0) // Elvis operator
```

---

## 👤 8. Classes and Objects

```kotlin
class Person(val name: String, var age: Int) {
    fun greet() {
        println("Hello, my name is $name and I'm $age")
    }
}
```

### Usage:

```kotlin
val person = Person("Alice", 25)
person.greet()
```

---

## 🧰 9. Collections

### List:

```kotlin
val list = listOf("Apple", "Banana", "Cherry")
val mutableList = mutableListOf("A", "B")
```

### Set:

```kotlin
val set = setOf(1, 2, 3, 2)
```

### Map:

```kotlin
val map = mapOf("name" to "John", "age" to 30)
val mutableMap = mutableMapOf("x" to 10)
```

---

## 🔧 10. Extensions

```kotlin
fun String.reverse(): String {
    return this.reversed()
}
println("Kotlin".reverse()) // "niltok"
```

---

## 🧵 11. String Templates

```kotlin
val name = "Sam"
println("Hello, $name!")  // Hello, Sam
```

---

## 🎯 12. Lambda Expressions

```kotlin
val sum = { a: Int, b: Int -> a + b }
println(sum(4, 5))
```

---

## 📚 13. Higher Order Function

```kotlin
fun operate(a: Int, b: Int, op: (Int, Int) -> Int): Int {
    return op(a, b)
}
val result = operate(4, 2) { x, y -> x * y }
```

---

## 📁 14. Data Classes

```kotlin
data class User(val name: String, val age: Int)

val u1 = User("Tom", 20)
println(u1.name)
```

---

## 🔄 15. Loop Ranges

```kotlin
for (i in 1..5) {}         // Inclusive
for (i in 1 until 5) {}    // Exclusive
for (i in 5 downTo 1) {}   // Reverse
for (i in 1..10 step 2) {} // Steps
```

---

## ✅ 16. Smart Casting

```kotlin
fun check(obj: Any) {
    if (obj is String) {
        println(obj.length) // smart cast
    }
}
```

---

## 🚨 17. Exception Handling

```kotlin
try {
    val num = 10 / 0
} catch (e: ArithmeticException) {
    println("Cannot divide by zero")
} finally {
    println("Done")
}
```

---

## 📦 18. Packages & Imports

```kotlin
package my.package.name

import kotlin.math.PI
```

---

## ✅ Summary: Must-Know Concepts

* Variables: `val`, `var`
* Data Types: `Int`, `String`, `Boolean`, etc.
* Null Safety: `?`, `?:`, `!!`
* Control Structures: `if`, `when`, loops
* Functions: `fun`, lambdas, HOFs
* Object-Oriented: `class`, `object`, `data class`
* Collections: `List`, `Map`, `Set`
* Kotlin is concise, null-safe, and interoperable with Java.

---

Happy coding! 🚀

```

---

Let me know if you want a downloadable version or a PDF of this!
```
