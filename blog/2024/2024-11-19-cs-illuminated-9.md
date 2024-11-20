---
layout: post
title: Chapter 9
author: Arpon Sarker
date: 2024-11-19 15:52:48
categories: [technology, coding]
tags: [compsci, programming, algorithms]
---

# Computer Science Illuminated Chapter 9 - Abstract Data Types and Algorithms

## Introduction
One of the various definitions of Computer Science is the study of algorithms and their efficient implementation. Abstract data types (ADT) are a data type whose properties are specified independently of any particular implementation. They are a container in which data items are stored in. *Data structures* are the actual implementations of these composite data fields in an ADT. 

## Implementation
The two implementations discussed here are the array-based implementation and the linked implementation. The array-based implementation are contiguously arranged cells of an array which is more efficient in searching through an array and uses a lesser length than the maximum given length of the actual array by the computer. A linked implementation consists of nodes and pointers and is much easier to insert and delete in this structure.

## Sorting
The three sorting algorithms talked about are the *selection sort*, *bubble sort* (especially useful for checking if list already sorted), and *quicksort*. Once the list is already sorted, we can use a much more efficient searching algorithm called *binary search* which eliminates large portions of data on each comparison.

## Stacks and Queues
A linked stack has insertions and deletions at the front whereas, a linked queue has deletions occuring at the front and insertions at a rear pointer.

## Binary Trees
A binary tree is a container object with a unique starting point called a *root* in which each node is capable of having two child nodes and a unique path exists from the root to every other node (no floating nodes). The *level* of a node refers to the distance from the root where level 0 is the root. The maximum number of levels is N. The maximum number of nodes in a tree is $2^{N+1}-1$. The minimum number of levels is $\log_2N+1$ levels.

A binary search tree shares the same property of a binary tree but each node's left subtree has values less than the node's value and each node's right subtree has values greater than the node's value. This combines the flexibility of a linked implementation of a list and the speed of binary search. This requires an *info* part and two pointers, one to the left subtree and another for the right subtree.

Graphs are a data structure that consists of a set of nodes and a set of edges that relate the nodes to each other. An *undirected graph* is a graph in which the edges have no direction and a *directed graph (digraph)* is one where each edge is directed from one vertex to another.
