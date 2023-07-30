# Learning Java
## What is Java?
- Java is a popular programming language, created in 1995.

- It is owned by Oracle, and more than 3 billion devices run Java.

- It is used for:
  - Mobile applications (specially Android apps)
  - Desktop applications
  - Web applications
  - Web servers and application servers
  - Games 
  - Database connection
   
 ## Why Use Java?
- Java works on different platforms (Windows, Mac, Linux, Raspberry Pi, etc.)
- It is one of the most popular programming language in the world
- It has a large demand in the current job market
- It is easy to learn and simple to use
- It is open-source and free
- It is secure, fast and powerful
- It has a huge community support (tens of millions of developers)
- Java is an object oriented language which gives a clear structure to programs and allows code to be reused, lowering development costs
- As Java is close to C++ and C#, it makes it easy for programmers to switch to Java or vice versa.
## Java Quickstart
- In Java, every application begins with a class name, and that class must match the filename.
```
public class Main {
  public static void main(String[] args) {
    System.out.println("Hello World");
  }
}
```
- Every line of code that runs in Java must be inside a class. 
- In our example, we named the class Main.
- A class should always start with an uppercase first letter.
- `Note:` Java is case-sensitive: "MyClass" and "myclass" has different meaning.
- The name of the java file must match the class name. 
- When saving the file, save it using the class name and add ".java" to the end of the filename. 

## The main Method
- The `main()` method is required and you will see it in every Java program:
```
public static void main(String[] args)
```
- Any code inside the `main()` method will be executed.

## System.out.println()
- Inside the `main()` method, we can use the `println()` method to print a line of text to the screen.
- You can add as many println() methods as you want. Note that it will add a new line for each method:
```
public static void main(String[] args) {
  System.out.println("Hello World");
}
```
- `System` is a built-in Java class that contains useful members, such as `out`, which is short for "output".
- The `println()` method, short for "print line", is used to print a value to the screen (or a file).
## The Print() Method
- There is also a print() method, which is similar to println().
- The only difference is that it does not insert a new line at the end of the output.
```agsl
System.out.print("Hello World! ");
System.out.print("I will print on the same line.");
```
## Print Numbers
- You can also use the println() method to print numbers.
 ```agsl
System.out.println(3);
System.out.println(358);
System.out.println(50000);
```
## Single-line Comments
- Single-line comments start with two forward slashes (//).
## Java Multi-line Comments
- Multi-line comments start with /* and ends with */.

- Any text between /* and */ will be ignored by Java.
```agsl
/* The code below will print the words Hello World
to the screen, and it is amazing */
System.out.println("Hello World");
```