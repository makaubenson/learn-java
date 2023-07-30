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
  - Reserved words (like Java keywords, such as int or boolean) cannot be used as names.

## Java Data Types
```agsl
int myNum = 5;               // Integer (whole number)
float myFloatNum = 5.99f;    // Floating point number
char myLetter = 'D';         // Character
boolean myBool = true;       // Boolean
String myText = "Hello";     // String
```
- Data types are divided into two groups:
  -  Primitive data types - includes byte, short, int, long, float, double, boolean and char
  - Non-primitive data types - such as String, Arrays and Classes (you will learn more about these in a later chapter)
- A `primitive data` type specifies the size and type of variable values, and it has no additional methods.
```agsl
Data Type	Size	Description
byte	    1 byte	Stores whole numbers from -128 to 127
short	    2 bytes	Stores whole numbers from -32,768 to 32,767
int	        4 bytes	Stores whole numbers from -2,147,483,648 to 2,147,483,647
long	    8 bytes	Stores whole numbers from -9,223,372,036,854,775,808 to 9,223,372,036,854,775,807
float	    4 bytes	Stores fractional numbers. Sufficient for storing 6 to 7 decimal digits
double	    8 bytes	Stores fractional numbers. Sufficient for storing 15 decimal digits
boolean	    1 bit	Stores true or false values
char	    2 bytes	Stores a single character/letter or ASCII values
```
## Java Numbers
- Primitive number types are divided into two groups:
  - Integer types stores whole numbers, positive or negative (such as 123 or -456), without decimals. Valid types are byte, short, int and long. Which type you should use, depends on the numeric value.
  - Floating point types represents numbers with a fractional part, containing one or more decimals. There are two types: float and double.
   
 ## Byte
- The byte data type can store whole numbers from -128 to 127. This can be used instead of int or other integer types to save memory when you are certain that the value will be within -128 and 127:
```agsl
byte myNum = 100;
System.out.println(myNum);
```
## Short
- The short data type can store whole numbers from -32768 to 32767:
```agsl
short myNum = 5000;
System.out.println(myNum);
```
## Int
- The int data type can store whole numbers from -2147483648 to 2147483647. In general, and in our tutorial, the int data type is the preferred data type when we create variables with a numeric value.
```agsl
int myNum = 100000;
System.out.println(myNum);
```
## Long
- The long data type can store whole numbers from -9223372036854775808 to 9223372036854775807. This is used when int is not large enough to store the value. Note that you should end the value with an "L":
```agsl
long myNum = 15000000000L;
System.out.println(myNum);
```
## Floating Point Types
- You should use a floating point type whenever you need a number with a decimal, such as 9.99 or 3.14515.
- The float and double data types can store fractional numbers. Note that you should end the value with an "f" for floats and "d" for doubles:
```agsl
float myNum = 5.75f;
System.out.println(myNum);
```

```agsl
double myNum = 19.99d;
System.out.println(myNum);
```
## Use float or double?

- The precision of a floating point value indicates how many digits the value can have after the decimal point.
- The precision of float is only six or seven decimal digits, while double variables have a precision of about 15 digits. 
- Therefore it is safer to use double for most calculations.

## Java Boolean Data Types
- Very often in programming, you will need a data type that can only have one of two values, like:
```
YES / NO
ON / OFF
TRUE / FALSE
```
- For this, Java has a boolean data type, which can only take the values true or false:
```agsl
boolean isJavaFun = true;
boolean isFishTasty = false;
System.out.println(isJavaFun);     // Outputs true
System.out.println(isFishTasty);   // Outputs false
```
## Java Characters
### Characters
- The char data type is used to store a single character. The character must be surrounded by single quotes, like 'A' or 'c':
```agsl
public class Main {
  public static void main(String[] args) {
    char myGrade = 'B';
    System.out.println(myGrade);
  }
}
```
### String
- The String data type is used to store a sequence of characters (text). String values must be surrounded by double quotes:
```
String greeting = "Hello World";
System.out.println(greeting);
```
## Java Non-Primitive Data Types
- Non-primitive data types are called reference types because they refer to objects.
- The main difference between primitive and non-primitive data types are:
  - Primitive types are predefined (already defined) in Java. Non-primitive types are created by the programmer and is not defined by Java (except for String).
  - Non-primitive types can be used to call methods to perform certain operations, while primitive types cannot.
   - A primitive type has always a value, while non-primitive types can be null.
    - A primitive type starts with a lowercase letter, while non-primitive types starts with an uppercase letter.
## Java Type Casting
- Type casting is when you assign a value of one primitive data type to another type.
- In Java, there are two types of casting:
  - Widening Casting (automatically) - converting a smaller type to a larger type size
    - `byte -> short -> char -> int -> long -> float -> double`
  - Narrowing Casting (manually) - converting a larger type to a smaller size type.
    - `double -> float -> long -> int -> char -> short -> byte`
 
   ### Widening Casting
- Widening casting is done automatically when passing a smaller size type to a larger size type:
``
```
public class Main {
  public static void main(String[] args) {
    int myInt = 9;
    double myDouble = myInt; // Automatic casting: int to double
    System.out.println(myInt);      // Outputs 9
    System.out.println(myDouble);   // Outputs 9.0
  }
}
```
### Narrowing Casting
- Narrowing casting must be done manually by placing the type in parentheses in front of the value:
```agsl
public class Main {
  public static void main(String[] args) {
    double myDouble = 9.78d;
    int myInt = (int) myDouble; // Manual casting: double to int
    System.out.println(myDouble);   // Outputs 9.78
    System.out.println(myInt);      // Outputs 9
  }
}
```
## Java Operators
- Operators are used to perform operations on variables and values.
- In the example below, we use the + operator to add together two values:
`int x = 100 + 50;`

```agsl
int sum1 = 100 + 50;        // 150 (100 + 50)
int sum2 = sum1 + 250;      // 400 (150 + 250)
int sum3 = sum2 + sum2;     // 800 (400 + 400)
```

- Java divides the operators into the following groups:
  - Arithmetic operators
  - Assignment operators
  - Comparison operators
  - Logical operators
  - Bitwise operators
```agsl
+	Addition	Adds together two values	x + y
```
```agsl
-	Subtraction	Subtracts one value from another	x - y
```

```agsl
*	Multiplication	Multiplies two values	x * y
```

```agsl
/	Division	Divides one value by another	x / y
```

```agsl
%	Modulus	Returns the division remainder	x % y
```

```agsl
++	Increment	Increases the value of a variable by 1	++x
```

```agsl
--	Decrement	Decreases the value of a variable by 1	--x
```

## Java Strings
- Strings are used for storing text. A String variable contains a collection of characters surrounded by double quotes:
`String greeting = "Hello";
## String Length
- A String in Java is actually an object, which contain methods that can perform certain operations on strings. For example, the length of a string can be found with the length() method:
```agsl
String txt = "ABCDEFGHIJKLMNOPQRSTUVWXYZ";
System.out.println("The length of the txt string is: " + txt.length());
```
## More String Methods
- There are many string methods available, for example `toUpperCase()` and `toLowerCase()`:
```agsl
String txt = "Hello World";
System.out.println(txt.toUpperCase());   // Outputs "HELLO WORLD"
System.out.println(txt.toLowerCase());   // Outputs "hello world"
```
- The indexOf() method returns the index (the position) of the first occurrence of a specified text in a string (including whitespace):
```agsl
String txt = "Please locate where 'locate' occurs!";
System.out.println(txt.indexOf("locate")); // Outputs 7
```

## Java String Concatenation
- The + operator can be used between strings to combine them. This is called concatenation:
```agsl
String firstName = "John";
String lastName = "Doe";
System.out.println(firstName + " " + lastName);
```
- You can also use the concat() method to concatenate two strings:
```agsl
String firstName = "John ";
String lastName = "Doe";
System.out.println(firstName.concat(lastName));
```

## Java Numbers and Strings
- Adding Numbers and Strings
- Java uses the + operator for both addition and concatenation.
- Numbers are added. Strings are concatenated.

```agsl
int x = 10;
int y = 20;
int z = x + y;  // z will be 30 (an integer/number)
```
- If you add two strings, the result will be a string concatenation:
```agsl
String x = "10";
String y = "20";
String z = x + y;  // z will be 1020 (a String)
```
- If you add a number and a string, the result will be a string concatenation:
```agsl
String x = "10";
int y = 20;
String z = x + y;  // z will be 1020 (a String)
```

## Java Special Characters
### Strings - Special Characters
- Because strings must be written within quotes, Java will misunderstand this string, and generate an error:
`String txt = "We are the so-called "Vikings" from the north.";`
- The solution to avoid this problem, is to use the backslash escape character.
- The backslash (\\) escape character turns special characters into string characters:

-  Single Quote
```agsl
\'	'	Single quote
```
- Double Quote
```agsl
\"	"	Double quote
```
- Backslash
```agsl
\\	\	Backslash
```
- Double Quote

```agsl
String txt = "We are the so-called \"Vikings\" from the north.";
```
-  Single quote
```agsl
String txt = 'It\'s alright.';
```
- Backslash
- `String txt = "The character \\ is called backslash.";`

```agsl
\n	New Line
\r	Carriage Return
\b	Backspace
\f	Form Feed
```

## Java Math
- The Java Math class has many methods that allows you to perform mathematical tasks on numbers.
- The `Math.max(x,y)` method can be used to find the highest value of x and y:
```agsl
public class Main {
  public static void main(String[] args) {
    System.out.println(Math.max(5, 10));  
  }
}
//10
```
- The Math.min(x,y) method can be used to find the lowest value of x and y:
```agsl
public class Main {
  public static void main(String[] args) {
    System.out.println(Math.min(5, 10));  
  }
}
//5
```
- The `Math.sqrt(x)` method returns the square root of x:
 ```agsl
public class Main {
  public static void main(String[] args) {
    System.out.println(Math.sqrt(64));  
  }
}
//8.0
```

- The Math.abs(x) method returns the absolute (positive) value of x:
```agsl
public class Main {
  public static void main(String[] args) {
    System.out.println(Math.abs(-4.7));  
  }
}
///4.7
```
- Math.random() returns a random number between 0.0 (inclusive), and 1.0 (exclusive):
```agsl
public class Main {
  public static void main(String[] args) {
    System.out.println(Math.random());  
  }
}
```
- To get more control over the random number, for example, if you only want a random number between 0 and 100, you can use the following formula:
```agsl
public class Main {
  public static void main(String[] args) {
    int randomNum = (int)(Math.random() * 101);  // 0 to 100
    System.out.println(randomNum);
  }
}
```

## Java Booleans
- A boolean type is declared with the boolean keyword and can only take the values true or false:
```agsl
boolean isJavaFun = true;
boolean isFishTasty = false;
System.out.println(isJavaFun);     // Outputs true
System.out.println(isFishTasty);   // Outputs false
```
- Example 2
```agsl
int x = 10;
int y = 9;
System.out.println(x > y); // returns true, because 10 is higher than 9
```

- Example 3
```agsl
System.out.println(10 > 9); // returns true, because 10 is higher than 9
```

- Real Life Example
```agsl
public class Main {
  public static void main(String[] args) {
    int myAge = 25;
    int votingAge = 18;
    
    if (myAge >= votingAge) {
      System.out.println("Old enough to vote!");
    } else {
      System.out.println("Not old enough to vote.");
    }  
  }
}
// Old enough to vote!
```

## Java If ... Else
### Java Conditions and If Statements
- You already know that Java supports the usual logical conditions from mathematics:
```agsl
Less than: a < b
Less than or equal to: a <= b
Greater than: a > b
Greater than or equal to: a >= b
Equal to a == b
Not Equal to: a != b
```
- Java has the following conditional statements:
  - Use `if` to specify a block of code to be executed, if a specified condition is true
  - Use `else` to specify a block of code to be executed, if the same condition is false
  - Use `else if` to specify a new condition to test, if the first condition is false
  - Use `switch` to specify many alternative blocks of code to be executed
 
## The if Statement
- Use the if statement to specify a block of Java code to be executed if a condition is true.
```agsl
if (condition) {
  // block of code to be executed if the condition is true
}
```
```agsl
public class Main {
  public static void main(String[] args) {
    if (20 > 18) {
      System.out.println("20 is greater than 18"); // obviously
    }  
  }
}
// 20 is greater than 18
```
- We can also test variables:
```agsl
public class Main {
  public static void main(String[] args) {
    int x = 20;
    int y = 18;
    if (x > y) {
      System.out.println("x is greater than y");
    }  
  }
}
//x is greater than y
```

## The else Statement
- Use the else statement to specify a block of code to be executed if the condition is false.
```agsl
if (condition) {
  // block of code to be executed if the condition is true
} else {
  // block of code to be executed if the condition is false
}
```
```agsl
public class Main {
  public static void main(String[] args) {
    int time = 20;
    if (time < 18) {
      System.out.println("Good day.");
    } else {
      System.out.println("Good evening.");
    }  
  }
}
//Good evening.
```
## The else if Statement
- Use the `else if` statement to specify a new condition if the first condition is false.
```agsl
if (condition1) {
  // block of code to be executed if condition1 is true
} else if (condition2) {
  // block of code to be executed if the condition1 is false and condition2 is true
} else {
  // block of code to be executed if the condition1 is false and condition2 is false
}
```

```agsl
public class Main {
  public static void main(String[] args) {
    int time = 22;
    if (time < 10) {
      System.out.println("Good morning.");
    } else if (time < 18) {
      System.out.println("Good day.");
    }  else {
      System.out.println("Good evening.");
    }
  }
}
//Good evening.
```

## Java Short Hand If...Else (Ternary Operator)
### Short Hand If...Else
- There is also a short-hand if else, which is known as the ternary operator because it consists of three operands.
- It can be used to replace multiple lines of code with a single line, and is most often used to replace simple if else statements:
```agsl
variable = (condition) ? expressionTrue :  expressionFalse;
```
- Instead of writing:
```agsl
public class Main {
  public static void main(String[] args) {
    int time = 20;
    if (time < 18) {
      System.out.println("Good day.");
    } else {
      System.out.println("Good evening.");
    }  
  }
}
//Good evening.
```
- You can simply write:
```agsl
public class Main {
  public static void main(String[] args) {   
    int time = 20;
    String result;
    result = (time < 18) ? "Good day." : "Good evening.";
    System.out.println(result);
  }
}
// Good evening.
```

## Java Switch Statements
- Instead of writing many if..else statements, you can use the switch statement.
- The `switch` statement selects one of many code blocks to be executed:
```agsl
switch(expression) {
  case x:
    // code block
    break;
  case y:
    // code block
    break;
  default:
    // code block
}
```
- This is how it works:
  - The switch expression is evaluated once.
  - The value of the expression is compared with the values of each case.
  - If there is a match, the associated block of code is executed.
  - The break and default keywords are optional, and will be described later in this chapter
 
- The example below uses the weekday number to calculate the weekday name:
```agsl
public class Main {
  public static void main(String[] args) {
    int day = 4;
    switch (day) {
      case 1:
        System.out.println("Monday");
        break;
      case 2:
        System.out.println("Tuesday");
        break;
      case 3:
        System.out.println("Wednesday");
        break;
      case 4:
        System.out.println("Thursday");
        break;
      case 5:
        System.out.println("Friday");
        break;
      case 6:
        System.out.println("Saturday");
        break;
      case 7:
        System.out.println("Sunday");
        break;
    }
  }
}
// Thursday
```

## The break Keyword
- When Java reaches a break keyword, it breaks out of the switch block.
- This will stop the execution of more code and case testing inside the block.
- When a match is found, and the job is done, it's time for a break. There is no need for more testing.
- A break can save a lot of execution time because it "ignores" the execution of all the rest of the code in the switch block.

## The default Keyword
- The `default` keyword specifies some code to run if there is no case match:
```agsl
public class Main {
  public static void main(String[] args) {
    int day = 4;
    switch (day) {
      case 6:
        System.out.println("Today is Saturday");
        break;
      case 7:
        System.out.println("Today is Sunday");
        break;
      default:
        System.out.println("Looking forward to the Weekend");
    }    
  }
}
//Looking forward to the Weekend
```
- Note that if the default statement is used as the last statement in a switch block, it does not need a break.

## Java While Loop
- Loops can execute a block of code as long as a specified condition is reached.
- Loops are handy because they save time, reduce errors, and they make code more readable.
### Java While Loop
- The while loop loops through a block of code as long as a specified condition is true:
```agsl
while (condition) {
  // code block to be executed
}
```

```agsl
public class Main {
  public static void main(String[] args) {
    int i = 0;
    while (i < 5) {
      System.out.println(i);
      i++;
    }  
  }
}
```

## The Do/While Loop
- The `do/while` loop is a variant of the while loop. 
- This loop will execute the code block once, before checking if the condition is true, then it will repeat the loop as long as the condition is true.
```agsl
do {
  // code block to be executed
}
while (condition);
```

- The example below uses a `do/while` loop. 
- The loop will always be executed at least once, even if the condition is false, because the code block is executed before the condition is tested:
```agsl
public class Main {
  public static void main(String[] args) {
    int i = 0;
    do {
      System.out.println(i);
      i++;
    }
    while (i < 5);  
  }
}

```