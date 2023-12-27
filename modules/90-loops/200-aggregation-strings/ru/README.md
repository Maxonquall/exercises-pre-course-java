Агрегация применяется не только к числам, но и к строкам.

При агрегации строка формируется динамически, то есть заранее неизвестно, какого она размера и что будет содержать. Представьте себе метод, который умеет умножать строку — то есть он повторяет ее указанное количество раз:

```java
App.repeat("hexlet", 3); // "hexlethexlethexlet"
```

Принцип работы этого метода довольно простой. В цикле происходит наращивание строки указанное количество раз:

```java
public static String repeat(String text, int times) {
    // Нейтральный элемент для строк – пустая строка
    var result = "";
    var i = 1;

    while (i <= times) {
        // Каждый раз добавляем строку к результату
        result = result + text;
        i = i + 1;
    }

    return result;
}
```

Распишем выполнение этого кода по шагам:

```java
// Для вызова repeat("hexlet", 3);
var result = "";
result = result + "hexlet"; // "hexlet"
result = result + "hexlet"; // "hexlethexlet"
result = result + "hexlet"; // "hexlethexlethexlet"
```
