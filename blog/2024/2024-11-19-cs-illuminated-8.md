---
layout: post
title: Chapter 8
author: Arpon Sarker
date: 2024-11-19 12:43:00
categories: [technology, coding]
tags: [compsci, programming, algorithms]
---

# Computer Science Illuminated Chapter 8 - High-Level Programming Languages

## Introduction
High-level languages were developed for a programmer to be able to communicate and think more complex ideas at a higher abstraction. 

## Translation Process
Compilers are a program that translates a high-level language program into machine code. Note that a machine-code version of the compiler must be available for a particular machine to be able to compile a program. Thus, to be used on multiple types of machines, each high-level language must have many compilers. 


Interpreters are a program that inputs a program in a high-level language and directs the computer to perform the actions specified in each statement. They can be viewed as simulators or virtual machines - executing the program directly. 

FORTRAN, COBOL, and ALGOL are compiled while Lisp, SNOBOL4, and APL are interpreted. The trend was towards the much faster compiled languages until Java (interpreted) came along. In the design of Java, portability was of utmost importance which was implemented by compiling its program into a standard machine language called *Bytecode*. For there to be a standard machine language on each machine, a JVM is needed which is a software interpreter that actually executes it. A program written on a compiled high-level language will need a machine that has the exact same compiler to run it, quite difficult on different OSs. However, a compiled Bytecode program can be run on any machine with a JVM interpreter.  

## Programming Language Paradigms
*Paradigm* - "*a set of assumptions, concepts, values, and practices that constitute **a way of viewing reality** for the community that shares them, especially in an intellectual discipline.*"
- Imperative/Procedural Model: allows the programmers to express algorithms as a hierarchy of tasks by sequential execution of instructions (unlike declarative nature of mathematics)
- Functional Model: computation is expressed in terms of evaluation of functions
- Logic Model: computation based on the the principles of symbolic logic, conisting of aksing questions based on objects and their relationships constrained by rules (e.g. PROLOG)
- Object-oriented Model: views computation as interacting objects, each responsible for its actions 

## Functionality of Imperative Languages
*Strong typing* enforces each variable to be assigned a type and only values of that type can be stored in the variable.
**Extra:** Dijkstra is much more known for his work in designing and advocating for structured programming rather than using jumps in assembly and opting for selection and iteration constructs. 

### Loops
*Count-controlled loops* is a loop that repeats a certain *number* of times whereas *Event-controlled loops* is a loop that repeats if some event's predicate is true where the event occurs within the loop of the body itself (e.g. reading a positive value in input which is used for next iteration's predicate). There are *pretest* loops which check the predicate first before entering a loop and *post-test* loops which execute the loop at least once before checking.

### Subprogram Statements
Subprograms here are labelled sections of code which can be referred to by some name and the place where this name appears is a *calling unit* (maybe similar to a function "call"). The two types are doing some task or doing some task and returning a value to the calling unit. 

A *value parameter* is a parameter taht expects a copy of its argument to be passed by the calling unit and a *reference parameter* expects the address of its argument to be passed by the calling unit. Recursion is the ability of a subprogram to call itself - some programs that are easier to be implemented by recursion may not be the right solution to do (run-time support system was also referenced here). 

*Asynchronous processing* is a specific operation in a computer such as a mouse click that does not occur at the same moment as some specific operation or with the computer's actions. This is also considered to be a control structure as this is an *instruction that controls the order of instructions executed*. 

Composite data types are a collection of date items together and are able to be accessed for each item individually (records and arrays). From SICP, this can be used as *glue* for creating more complex abstract data types. 

## Functionality of Object-Oriented Languages
- Encapsulation: bundling of data and actions such that the logical properties of the data and actions remain separate from the implementation details. This enforces information hiding. 
- Inheritance: a mechanism in which one class acquires the data fields and methods of another class. Able to add onto the inherited properties for its own specific functionality.
- Polymorphism: the ability of a language to have duplicate method names and to apply the appropriate method for the object on which it is applied to.

