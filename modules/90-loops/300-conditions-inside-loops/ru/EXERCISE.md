
Метод из теории учитывает регистр букв. То есть `A` и `a` с его точки зрения разные символы. Реализуйте вариант этого же метода, так чтобы регистр букв был не важен:

```java
App.countChars("HexlEt", 'e'); // 2
App.countChars("HexlEt", 'E'); // 2
```

* `Character.toLowerCase()` – переводит символ в нижний регистр