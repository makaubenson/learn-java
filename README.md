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

## Java Variables
- Variables are containers for storing data values.
- In Java, there are different types of variables, for example:
  - String - stores text, such as "Hello". String values are surrounded by double quotes
   - int - stores integers (whole numbers), without decimals, such as 123 or -123
   - float - stores floating point numbers, with decimals, such as 19.99 or -19.99
   - char - stores single characters, such as 'a' or 'B'. Char values are surrounded by single quotes
   - boolean - stores values with two states: true or false.
  
## Declaring (Creating) Variables
- To create a variable, you must specify the type and assign it a value:
`type variableName = value;`
- e.g
```agsl
String name = "John";
System.out.println(name);

int myNum = 15;
System.out.println(myNum);
```
- You can also declare a variable without assigning the value, and assign the value later:
```agsl
int myNum;
myNum = 15;
System.out.println(myNum);
```

## Final Variables
- If you don't want others (or yourself) to overwrite existing values, use the final keyword (this will declare the variable as "final" or "constant", which means unchangeable and read-only):
```agsl
final int myNum = 15;
myNum = 20;  // will generate an error: cannot assign a value to a final variable
```
## Display Variables
- The println() method is often used to display variables.
- To combine both text and a variable, use the + character:
```agsl
String name = "John";
System.out.println("Hello " + name);
```

```agsl
String firstName = "John ";
String lastName = "Doe";
String fullName = firstName + lastName;
System.out.println(fullName);
```

## Java Identifiers
- All Java variables must be identified with unique names.
- These unique names are called identifiers. 
- Identifiers can be short names (like x and y) or more descriptive names (age, sum, totalVolume).
- Note: It is recommended to use descriptive names in order to create understandable and maintainable code:
```agsl
// Good
int minutesPerHour = 60;

// OK, but not so easy to understand what m actually is
int m = 60;
```

### The general rules for naming variables are:
  - Names can contain letters, digits, underscores, and dollar signs 
  - Names must begin with a letter 
  - Names should start with a lowercase letter and it cannot contain whitespace 
  - Names can also begin with $ and _ (but we will not use it in this tutorial)
  - Names are case sensitive ("myVar" and "myvar" are different variables)
  - Reserved words (like Java keywords, such as int or boolean) cannot be used as names