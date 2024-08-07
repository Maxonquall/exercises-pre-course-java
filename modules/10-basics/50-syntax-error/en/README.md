In human languages, grammar is important, but text with errors can most often be understood and read. In programming, everything is strict. Any tiny violation and the program will not run.

An example is a forgotten `;`, misplaced parentheses, and other details. Such errors are called **syntactic** because they violate the syntax rules of the language.

If a Java program is written syntactically incorrect, the compiler displays:

* An error message
* A pointer to a file
* The line in the file where it thinks the error occurred

Below is an example of code with a syntax error:

```java
System.out.println("alala
```

If we run the code above, we see the following message:

<pre class='hexlet-basics-output'>
| Error:
| unclosed string literal
| System.out.println("alala
</pre>

On the one hand, syntax errors are the simplest ones because they are related only to grammatical rules of code writing and not to the meaning of the code itself. They are easy to fix - you just need to find a violation in the record.

On the other hand, the compiler cannot always clearly point out this violation. That's why it happens that a forgotten parenthesis must be placed in a different place than the error message indicates.