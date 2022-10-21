# Day Five

# Q1. 
    - Explain what it means by:
        - loosely typed dynamic language
        - JavaScript Type Casting
        - ==, ===
## A1
    Loosely typed dynamic language:
        A Loosely typed programming language is defined as a language where defining a variable's data type is not requiredd.
    
    JavaScript Type Casting:
        
    
    ==, ===
        - Double equals used as Type converting the conversion.
        - Triple equals used as Strict conversion without performing any conversion in operands.
    
# Q2
    - Answer the following questions:
        - What is the problem of a loosely typed dynamic language, and what are the ways to supplement it?
        - Compare the difference between undefined and null.

## A2
    - The problem of a loosely typed dynamic language:
        One of the problems of a loosely typed dynamic langguage is produce Unexpected results, to supplement it we can use any methods of JS. Such as adding int() to declare the integer value, String() to supplement type for string.
    
    - The difference between undefined and null:
        Null is usually obtained under normal and planned conditions. However undefined is usually obtained from the result of a program error and is not planned.

# Q3
    - Explain what it means by:
        - Primitive type data, and Reference type data.
        - JavaScript Type Casting

## A3
    Primitive type data:
        Primitive data type - is a basic data type that is available directly in a programming language. For example integer and char data types.
    
    Reference type data:
        Non-primitive data types are known as reference types, a variable of class type is called reference data type. It contains the address (or reference) of dynamically created objects. For example, if Demo is a class and we have created its object d, then the variable d is known as a reference type.

    JS type casting:
        Type casting means conversion of one data type to another explicitly. In JavaScript some of the most common methods to convert a datatype to either string using String (), to boolean using Boolean (), or to number using Number ().

# Q4
    - Answer the following questions:
        - How to make Immutable Object?
        - What are shallow copy and deep copy. What are the differences?

## A4
    How to make Immutable Object:
        Object Assign() is a command to copy an object to a new object complete with its reference and value. With this command the target object no longer uses the same value as the old object.

    Shallow copy: reflects the changes made to the new/copied object in the original object. Shallow Copy stores a copy of the original object and points a reference to the object.

    Deep Copy: copy stores a copy of the value object. The deep copy does not reflect changes made to the new object/copy in the original object.

# Q5
    - Explain what it means by:
        - Scope, Hoisting and TDZ
        - Different ways of hoisting in Function Declarations and Function Expressions.
        - Execution Context and Call Stack
        - Scope Chain and Information Hiding

## A5
    Scope in JavaScript is a concept used to limit access to a variable. There are two types of scopes, namely local and global.
        Global variables are variables declared outside the block.
        Local variables are variables declared inside a block can be either function-scoped or block-scoped.
    
    Hoisting: Hoisting will only move up the scope of a variable declaration not its initiation.

    TDZ: Temporal Dead Zone explained This is what the TDZ is: the term to describe the state where variables are un-reachable. They are in scope, but they aren't declared.

    Function declarations have been used for a long time, but function expressions have been gradually taking over.
    Ex: 
        function funcDeclaration() {
            return 'A function declaration';
        }

        let funcExpression = function () {
            return 'A function expression';
        }

    Execution context is the environment that enables JavaScript code to execute. It decides which piece of code currently gets access to all the functions, variables and objects used in the code for its execution.

    Call Stack is a data-structure that maintains the list of the functions being called and executed/ the execution context currently being executed by the JavaScript engine.

    Scope Chain:
        When a variable is used in JavaScript, the JavaScript engine will try to find the variable’s value in the current scope. If it could not find the variable, it will look into the outer scope and will continue to do so until it finds the variable or reaches global scope.

        If it’s still could not find the variable, it will either implicitly declare the variable in the global scope (if not in strict mode) or return an error.

    Information Hiding:
        Refers to the practice of concealing implementation details that are unfit for the consumers of the code.

```
let b = 1;

function hi () {

const a = 1;

let b = 100;

b++;

console.log(a,b);

}

//console.log(a);

console.log(b);

hi();

console.log(b);
```