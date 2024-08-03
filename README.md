# Kotlin Practice Programs

This repository contains Kotlin programs that perform various tasks such as drawing shapes, counting vowels, 
reversing strings, filtering digits, splitting strings into words, and removing spaces from strings.

### Drawing a Right-Angled Triangle 
* This program draws a right-angled triangle of stars with a height of 5.

    ```diff
     for (index in 1..5) {
        for (item in 1..index) {
            print("*")
        }
        println(" ")
    }
    ```

#### Result 
  <img src="https://github.com/MohammedAgamy/TaskSession3/blob/master/1.jpg"  width="400" high="100">

### Drawing an Isosceles Triangle
* This program draws an isosceles triangle of stars with a height of 5.
```diff
 for (index in 1..5) {
        for (i in 5 downTo index) {
            print("  ")
        }
        for (item in 1..<index * 2) {
            print(" ")
            print("*")
        }
        println()
    }
```
#### Result 
  <img src="https://github.com/MohammedAgamy/TaskSession3/blob/master/2.jpg"  width="400" high="100">
  
### Drawing a Pyramid
* This program draws a pyramid of stars with a height of 5.

```diff
     var height = 5

    for (index in 1..height) {
        for (i in 1..height - index) {
            print(" ")
        }
        for (item in 1..(2 * index - 1)) {
            print("*")
        }

        println()
    }
```

#### Result 
  <img src="https://github.com/MohammedAgamy/TaskSession3/blob/master/3.jpg"  width="400" high="100">

  
### Counting Vowels in a String
* This program counts the number of vowels (a, e, i, o, u) in the string "Kotlin is awesome".

```diff
         var sum: Int? = null
    val counts = "Kotlin is awesome"
    for (i in counts) {
        if (i == 'o' || i == 'e' || i == 'i' || i == 'a' || i == 'u') {
            println(i)
            sum = (sum ?: 0) + 1
        }
    }
    println("counts the number of vowels $sum")
```
#### Result 
  <img src="https://github.com/MohammedAgamy/TaskSession3/blob/master/4.jpg"  width="400" high="100">

  
### Reversing a String
* This program reverses the string "Kotlin".

  ```diff
  var kotlinVal = "Kotlin"
    println(kotlinVal.reversed())
    /*another way */
    for (item in kotlinVal.reversed()) {
        println(item)
    }
    println("counts the number of vowels $sum")
  ```

  <img src="https://github.com/MohammedAgamy/TaskSession3/blob/master/5.jpg"  width="400" high="100">

### Filtering Digits from a String
* This program filters and prints only the digits from the string "K0t1l1n 2s 4w3s0m3".

  ```diff
  var text = "K0t1l1n 2s 4w3s0m3"
    for (item in text.filter { it.isDigit() }) {
        println(item)
    }

    /*another way */
    val digit = text.filter {
        it.isDigit()
    }
  ```
  <img src="https://github.com/MohammedAgamy/TaskSession3/blob/master/6.jpg"  width="400" high="100">
  
### Splitting a String into Words && Counting Words in a String
* This program splits the string "Kotlin is a great language" into words and prints each word on a new line.
* Write a Kotlin program that counts the number of words in the string "Kotlin is a great language
    ```diff
   var count: Int? = null
    var splitting = "Kotlin is a great language"
    val sPilt = splitting.split(" ")
    for (item in sPilt) {
        println("word $item")
        count = (count ?: 0) + 1
    }

    println(count)
   ```
  <img src="https://github.com/MohammedAgamy/TaskSession3/blob/master/7.jpg"  width="400" high="100">

### Removing Spaces from a String
* This program removes all spaces from the string "Kotlin is fun" and prints the result.
```diff
  val funk = "Kotlin is fun"
    val replace = funk.replace(" ", "")
    println(replace
```

<img src="https://github.com/MohammedAgamy/TaskSession3/blob/master/8.jpg"  width="400" high="100">

