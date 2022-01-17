# Java #
- Java was originally designed for programming consumer devices but it's success came from writing internet applets.
- Java is both **safe** and **portable**

## Java Compiler ##
- Java source code is transalted into **byte-code**
- A machine language for a fictious computer called the **JVM**
- **Example**: asking a **translator** to translate english text into french.
- A compiler is a progfram that translates high level instructions into more detailed instructions that can be exceuted by the CPU

## Java Interpreter ##
- Exectutes **JVM**
- Transalted byte-code into machine language and executes it
- Translating byte-code into machine code is relatevily easy comapred to the itnial compilation step
*byte code is already close to machine language*
**Note:** Once compiled to byte-code a Java program can be used on any computer making it very portable

## Flowchart ##
- Java source code (`MyProg.java`) -> *Compiler* -> Java byte code (`MyProg.class`) -> *Interpreter* -> Machine code

## 3 types of errors ##
1. Compile-time (syntax) errors
    - The compiler will find syntax errors and basic problems
    -An executable version of the program is **not** created
2. Run-time errors
    - During a program execution
    - causes programs to terminate abnormally
    - **Example**: Divide by zero
3. Logical (semantic) erros
    - AKA a bug
    - mistake in the algorithm
    - compiler can't catch them
    - the program will run but will give unexpected results
- Compile and Run-time errors are easy to debug
- Logical errors are harder to debug

## Boilerplate for any `.Java` file ##
```
public class ClassName
{
  public static void main(String[] args)
  {
    ...
  }
}
```

## Algorithm ##
- An algorithm is:
    1. unambigous
    2. executable
    3. terminating

## System.out.println ##
- For them example of `System.out.println("blabla")`, the string "blabla" will be printed first **and then** the cursor is placed to the next line

## Comments ##
- Comments can take 3 forms:
1. `//` this commentruns to the end of the line
2. `/* */` the comment runs to the terminating symbol, even across line breaks
3. `/** */` use to make JavaDoc comments

## Indentifiers ##
- The words a programmer uses in a program to name variables, classes and methods
- It can cotnain letters, digits and underscores
- it **can't** have a reserved word (*note: all reserved words are lowercase)
- Limit length ex: numberOfCoffees can be nbOfCoffees
1. ### Guidelines ###  
- Give a significant name
- Avoid using the "$" sign
2. ### Conventions ###
- Class names should be titleCase -> `MyClass`
- constants should be uppercase -> `MAXIMUM`
- variables, methods should start with lowercase -> `firstName`

## Indentation ##
- extra white space is ignored
- Programs should be formatted to enhance readability using consostent indentation

## Primative types ##
1. Numeric
    - 4 types of integers: `byte, short, int, long`
    - 2 types to represent floating point numbers (ex: 3.5) `float, double` 
      - floating points are approximate values
2. Characters
    - `char` ex: 'a' 
    - Java uses the unicod3e character set. ASCII is a sub-set of Unicode
3. Boolean
    - `boolean` ex: `true` or `false`

## Variables ##
- A name for a location in memory
- must be declared before it is used
- indicate variable's name, indicate the type of information it will contain
- Uninitialized variable -> `int total;` 
- Initialized variable -> `int max = 150;` 

## Constants ##
- Similar to a variable but can hold only one value while the program is active
- the compiler will cause an error if you try to change the value of a constant during execution
- use the `final` modifierex: `final int MIN_AGE = 18;`

## Scanner ##
- Close the scanner with `scanner.close()`
- good habit to close the scanner object at the end of the main method in your program

## print and println ##
- the "+" if for concatenation
- you need parenthesis for the "+" to be an addition
- example:
```
int x = 1;
int y = 2;
System.out.println("x+y=" + x + y) // "x+y=12"
System.out.println("x+y=" + (x + y)) // "x+y=2"
```
## Operator associativity ##
- A string of assignment operators is grouped right to left
- ex: `n1 = n2 = n3` is evaluated as `n2 = n3` and then `n1 = n2`

## Increment and decrement ##
1. Prefix form: `++count`
    - the variable is inc/dec by 1 **THEN** the new value of the variable is used
2. Postfix form: `count++`
    - the variable is used with it's current value **THEN** the variable is inc/dec by 1

## Arithmetic Promotion ##
```
byte -> short and char -> int -> long -> float -> double
```
- **NOTE**: `byte + byte = int` because a byte automatically gets promoted to an integer
- **NOTE**: booleans are not compatible with any type

## Casting ##
- The programmer can explicitly force a type conversion by casting
- syntax: `(desired_type) expression_to_convert`
```
int num;
num = (int) 3.7  //num = 3
```
```
double d;
d = 2 / 4                          //d is 0.0
d = (double) 2 / 4                 //d is 0.5 since the 2 becomes a 2.0
d = (double) (2 / 4)               //d is 0.0 since (2 / 4) is evaluted first at that evaluates to 0
```