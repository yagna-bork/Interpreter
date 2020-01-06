# Interpreter for non-negative calculations

This interpreter allows you to write code that performs addition, multiplication, order of operations, parenthesis, function definition and function calling with arguments for non-negative integers

# Syntax

Every program must:

* Must define MAIN()
* DEF MAIN { A(1) } ; //valid main function
* DEF A x { x+1 } ; //valid function with parameter
* FUNCTION NAMES ARE UPPER CASE
* parameters are lower case
* ~~1.0,2.1,-3~~ are invalid
* ~~-, /~~ are invalid operations
* Functions being called must be defined
* Interpreter can detect infinite left and right recursion and prints `DIVERGENCE` to stdout

# How do I run it?
## Dependencies

* [Javacc](https://javacc.github.io/javacc/) (Put in same file as Interpreter.jj) 
* Java

## Steps

1. Create interpreter: `javacc-6.0/bin/javacc Interpreter.jj`
2. Compile java classes: `javac *.java`
3. Run test files: `java Interpreter < tests/validFiles.txt`
4. Your code just got interpreted!
