Here are some **basic Kotlin programs** that demonstrate key concepts like **variables, data types, conditions, loops, functions, classes, null safety, and collections**. These programs will help you get hands-on with the Kotlin basics.

---

### 📌 1. Print Hello World

```kotlin
fun main() {
    println("Hello, World!")
}
```

---

### 📌 2. Add Two Numbers

```kotlin
fun main() {
    val a = 10
    val b = 20
    val sum = a + b
    println("Sum = $sum")
}
```

---

### 📌 3. Check Even or Odd

```kotlin
fun main() {
    val num = 5
    if (num % 2 == 0) {
        println("$num is Even")
    } else {
        println("$num is Odd")
    }
}
```

---

### 📌 4. Find Maximum of Two Numbers

```kotlin
fun main() {
    val a = 15
    val b = 10
    val max = if (a > b) a else b
    println("Max = $max")
}
```

---

### 📌 5. When Expression (Switch Case)

```kotlin
fun main() {
    val day = 3
    val dayName = when(day) {
        1 -> "Monday"
        2 -> "Tuesday"
        3 -> "Wednesday"
        else -> "Invalid Day"
    }
    println(dayName)
}
```

---

### 📌 6. For Loop (Print 1 to 5)

```kotlin
fun main() {
    for (i in 1..5) {
        println(i)
    }
}
```

---

### 📌 7. Function to Calculate Factorial

```kotlin
fun factorial(n: Int): Int {
    var result = 1
    for (i in 1..n) {
        result *= i
    }
    return result
}

fun main() {
    val num = 5
    println("Factorial of $num = ${factorial(num)}")
}
```

---

### 📌 8. Class and Object Example

```kotlin
class Person(val name: String, val age: Int) {
    fun displayInfo() {
        println("Name: $name, Age: $age")
    }
}

fun main() {
    val p = Person("Alice", 22)
    p.displayInfo()
}
```

---

### 📌 9. Null Safety Example

```kotlin
fun main() {
    var name: String? = null
    println(name?.length ?: "Name is null")
}
```

---

### 📌 10. Use of List and Loop

```kotlin
fun main() {
    val fruits = listOf("Apple", "Banana", "Mango")
    for (fruit in fruits) {
        println(fruit)
    }
}
```

---

### 📌 11. Lambda Function Example

```kotlin
fun main() {
    val square = { x: Int -> x * x }
    println("Square of 4 = ${square(4)}")
}
```

---

### 📌 12. Higher Order Function Example

```kotlin
fun operate(a: Int, b: Int, operation: (Int, Int) -> Int): Int {
    return operation(a, b)
}

fun main() {
    val sum = operate(5, 3) { x, y -> x + y }
    println("Result = $sum")
}
```

---

### 📌 13. String Templates Example

```kotlin
fun main() {
    val name = "Kotlin"
    val version = 1.8
    println("Language: $name, Version: $version")
}
```


