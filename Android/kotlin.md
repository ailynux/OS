# Kotlin for <img src="https://user-images.githubusercontent.com/74038190/212281763-e6ecd7ef-c4aa-45b6-a97c-f33f6bb592bd.gif" width="100">

## Welcome to my notes! 
<img src="https://user-images.githubusercontent.com/74038190/215768208-3bf3dda8-eeea-40ee-a58b-f5ac529685bf.gif" width="900">

## Table of Contents
- [Prerequisites](#prerequisites)
- [Installation](#installation)
- [Hello World](#hello-world)
- [Basic Arithmetic Operators](#basic-arithmetic-operators)

## Prerequisites

Before you start, make sure you have the following prerequisites installed on your machine:
- Java Development Kit (JDK) 8 or later
- IntelliJ IDEA or any other preferred Kotlin IDE
- Android Studio
- Online Playgrounds

## Installation

To start using Kotlin, you can either use the Kotlin command-line compiler or an IDE like IntelliJ IDEA. 
1. Download and install IntelliJ IDEA: [IntelliJ IDEA](https://www.jetbrains.com/idea/download/)
2. **Download and Install Android Studio:** [Android Studio](https://developer.android.com/studio)

   Android Studio is the official IDE for Android development. Download and install it by following the instructions on the official website.

   - Launch Android Studio after installation.
   - Configure the Android SDK and other settings as prompted during the first launch.

## Hello World

Let's start with a classic "Hello World" example in Kotlin. Create a new Kotlin file, typically with a `.kt` extension.

```kotlin
// HelloWorld.kt
fun main() {
    println("Hello, Kotlin!")
}
```
## Basic Arithmetic Operators

Kotlin supports standard arithmetic operators for numeric types. Here's a quick reference:

| Operator | Description      | Example    |
|----------|------------------|------------|
| `+`      | Addition         | `a + b`    |
| `-`      | Subtraction      | `a - b`    |
| `*`      | Multiplication   | `a * b`    |
| `/`      | Division         | `a / b`    |
| `%`      | Modulus (Remainder) | `a % b`  |

```kotlin
// ArithmeticOperators.kt
fun main() {
    val a = 10
    val b = 3

    val sum = a + b
    val difference = a - b
    val product = a * b
    val quotient = a / b
    val remainder = a % b

    println("Sum: \$sum")
    println("Difference: \$difference")
    println("Product: \$product")
    println("Quotient: \$quotient")
    println("Remainder: \$remainder")
}
```
# Kotlin Programming Notes

## Table of Contents
- [Nullable Types](#nullable-types)
- [String Templates](#string-templates)
- [Collections](#collections)
- [Functions](#functions)
- [Classes and Objects](#classes-and-objects)

## Nullable Types
In Kotlin, variables are non-nullable by default. If you want to allow null values, you can use the nullable type modifier `?`.

```kotlin
var nullableString: String? = null
```
## String Templates
Kotlin supports string templates, allowing you to embed expressions directly in strings.

```kotlin
val name = "John"
val greeting = "Hello, $name!"
println(greeting)
```
## Collections 
Kotlin provides a rich set of collection types, including lists, sets, and maps.

```kotlin
//list
val numbers = listOf(1, 2, 3, 4, 5)
println(numbers)
```
```kotlin
//set
val uniqueNumbers = setOf(1, 2, 3, 4, 5)
println(uniqueNumbers)
```
```kotlin
//map
val userMap = mapOf("name" to "Ailyn", "age" to 22)
```

## Functions
Functions in Kotlin are defined using the `fun` keyword. They can have parameters and a return type.

```kotlin
fun add(a: Int, b: Int): Int {
    return a + b
}

val result = add(3, 7)
println("Result: $result")
```

## Classes and Objects
Kotlin supports both object-oriented and functional programming paradigms. Here's a simple example of a class:

```kotlin
class Person(val name: String, val age: Int)

val person = Person("Ailyn", 22)
println("Name: ${person.name}, Age: ${person.age}")
```


# Advanced Kotlin 
 These notes cover more sophisticated features and techniques to enhance your Kotlin skills.

## Table of Contents
- [Coroutines](#coroutines)
- [Extension Functions](#extension-functions)
- [Data Classes](#data-classes)
- [Destructuring Declarations](#destructuring-declarations)
- [Sealed Classes](#sealed-classes)

## Coroutines
Kotlin provides support for coroutines, enabling asynchronous programming without the complexity of traditional threads.

```kotlin
import kotlinx.coroutines.*

fun main() = runBlocking {
    launch {
        delay(1000L)
        println("World!")
    }
    println("Hello, ")
}
```
## Extension Functions
Extension functions allow you to add new functions to existing classes without modifying their code.

```kotlin
fun String.toTitleCase(): String {
    return this.split(" ").joinToString(" ") { it.capitalize() }
}

val title = "kotlin programming".toTitleCase()
println(title)
```
## Data Classes 
Data classes in Kotlin are concise and powerful, automatically generating essential methods like toString(), equals(), and hashCode().
```kotlin
data class Person(val name: String, val age: Int)

val person1 = Person("Alice", 30)
val person2 = Person("Alice", 30)

println(person1 == person2)  // true
```
## Destructuring Declarations
Destructuring declarations allow you to break down objects into their component parts.

```kotlin
val (name, age) = person1
println("Name: $name, Age: $age")
```
## Sealed Classes  
Sealed classes are a powerful tool for modeling restricted class hierarchies. They are often used in conjunction with when expressions.

```kotlin
sealed class Result {
    data class Success(val data: String) : Result()
    data class Error(val message: String) : Result()
}

val result: Result = Result.Success("Data received")

when (result) {
    is Result.Success -> println("Success: ${result.data}")
    is Result.Error -> println("Error: ${result.message}")
}
```
These advanced Kotlin features offer powerful solutions for complex programming scenarios.

