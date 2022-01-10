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
