# Interpreter for non-negative calculations

This interpreter allows you to write code that performs addition, multiplication, order of operations, parenthesis, function definition and function calling with arguments for non-negative integers

# Syntax

Every program must:

* Define a main function
* Main function must return a valid  
* Only non-negative integers, function call, multiplication and addition are valid syntax
* Functions being called must be defined
* Program can detect infinite left and right recursion and throws a `DIVERGENCE` error

# How do I run it?
## Dependencies

* Javacc: [Download](https://javacc.github.io/javacc/)
* Java

## Steps

1. Create interpreter: `javacc-6.0/bin/javacc Interpreter.jj`
2. Compile java classes: `javac *.java`
3. Run test files: `java Interpreter < tests/validFiles.txt`
4. Your code just got interpreted!
