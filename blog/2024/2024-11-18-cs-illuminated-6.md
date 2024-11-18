---
layout: post
title: Chapter 6
author: Arpon Sarker
date: 2024-11-18 20:17:30
categories: [technology, coding]
tags: [compsci, programming, algorithms]
---

# Computer Science Illuminated Chapter 6 - Problem Solving and Algorithm Design

## Introduction
The idea of problem solving and algorithm design is fundamentally important in all facets of life especially in computer science but getting better at this can only be done with practice. This chapter goes over Polya's problem solving process and looks at top-down vs object-oriented design methodologies.

## How to Solve It
George Polya wrote How to Solve It in 1945 which was written when computers were still experimental and was targeted for mathematics.

- Understanding the Problem (What is the unknown, data, and condition?)
- Devising a Plan (Have you seen it before? Could you introduce an auxiliary element?)
- Carrying out the Plan (Check each step)
- Looking Back (Can you check the result? Can you see it at a glance? Can you derive it differently?)

## Developing an Algorithm

### Top-Down Design Methodology
This process starts by breaking down the problem into subproblems and those subproblems are broken down until each subproblem is defined at a basic level. An *abstract step* is a step that needs to be expanded and a *concrete step* is a step that doesn't need to be expanded. 

### Object-Oriented Methodology
Top-Down design methodology focuses on the procedures to solve a problem whereas, object-oriented methodology focuses on the objects and their interactions (containing both data and operations that manipulate data in self-contained entities) to solve the problem. A group of similar objects is defined a class. Furthermore, *information hiding* is deferring the details until they are implemented later and not be bogged down by the lower abstractions. Information hiding is the practice of hiding details and *abstraction* is the result of this. *Data abstraction* is the separation of the logical view of the data from its implementation. *Procedural abstraction* is the separation of the logical view of an action from its implementation. *Control abstraction* is the separation of the logical view of a control structure from its implmentation (whiles and ifs). 
