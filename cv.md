# CV
## Contact info:
Hello, I'm [Alexandr Popko](https://vk.com/id178051637)
- Discord: ProstoSasha0612#4945
- [Github](https://github.com/ProstoSasha0612)
- Telegram: Mr_Sasha0
- [LinkedIn](https://www.linkedin.com/in/александр-попко-98605a1b2/)

## Short bio:
I'm a student of the it-university called BSUIR, and like Android-development. 
I learn Android, because Android it's very intresting platform.
I'm a 2nd year student at the university. 3 months of studying C# | then 6 months of studying Java/Kotlin and working with Andoid Studio.
I read the "Herbert Shildt C#", "Herbert Schildt Java", "Kotlin in Action". I completed the Udemy courses Java, Kotlin and Stepik course Kotlin

## My skills:
Java and Kotlin
Good knowledge on VCS Git, Algorithm, Data Structure, 
IDE Intelllij Idea and Android Studio, OOP, Lambda, base knowledges of concurency,JVM, etc.
My english level about A2.

## Example of solved task
```kotlin
fun main() {
    val input = readLine() ?: "Nothing"
    val inputList = input.split(" ").sorted()
    val res = sortLists(inputList)

    for (i in res) { 
        for (j in i) {
            print(j + " ")
        }
        println()
    }
}

fun sortLists(inputList: List<String>): MutableList<MutableList<String>> {
    val res = mutableListOf<MutableList<String>>()
    var counter = 0
    for (i in inputList) {
        if (res.isEmpty()) {
            res.add(mutableListOf(i))
            continue
        }
        if (i[0] == res[counter][0][0]) {
            res[counter].add(i)
        } else {
            res.add(mutableListOf())
            res[++counter].add(i)
        }
    }
    return res
}
```
