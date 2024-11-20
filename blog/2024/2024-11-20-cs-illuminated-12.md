---
layout: post
title: Chapter 12
author: Arpon Sarker
date: 2024-11-20 18:50:24
categories: [technology, coding]
tags: [compsci, programming, algorithms]
---

# Computer Science Illuminated Chapter 12 - Information Systems

## Introduction
I have only ever interacted with computers at the application layer for most of my life and have recently done high-level languages and for one course have done assembly and logic gates. General information systems manage everything in all sorts of industries such as banking, statistics, and business analytics. An *information system* is software that helps the user organise and analyse data.

## Spreadsheets
*Spreadsheets* are a program that allows th user to organise and analyse data using a grid of cells. Data stored in a cell can be text, numbers or "special data" such as dates. Usually text is just labels to further inform what the data is about which could be anything which is why spreadsheets are so flexible for application in many domains. The great thing about spreadsheets is that they are easily scalable and formulas used will automatically incorporate the newly added data based on the range of cells given. However, circular references can be made where cells rely on values from each other. For *spreadsheet analysis*, what-if? analysis is used where changing a couple of variables that represent assumptions to see how those changes affect related data.


## Database Management Systems
A *database* (DB) is a structured set of data. A *database management system* (DBMS) is a combination of software and data made up of the physical database, the database engine (software that supports access to and modification of the DB contents for the user), and the database schema (a specification of the logical structure of the data stored in a DB). The *relational model* is the most popular DB management models in which data and the relationships among them are organised into tables. *Records* are a collection of related fields that make up a database entry and a *field/attribute* is a single value in a record.

*Structued Query Language* (SQL) is a comprehensive database language for managing relational databases and includes the ability to specify database schemas; add, modify, and delete database content; and query to retrieve specific data. 

Database design must be carefully done at the start to capture all the required relationships. One popular technique is *entity-relationship* (ER) modeling with an *ER diagram* which captures the important record types, attributes, and relationships in a graph and includes cardinality constraints for relationships. 

## Information Security
Information security can be described as a culmination of *confidentiality*, *integrity*, and *availability*. Confidentiality is ensuring the data is protected from unauthorised access. Integrity ensures that the data can only be modified by appropriate mechanisms and availability is the degree to which authorised users can access information for legitimiate purposes. A *risk analysis* must be conducted to determine the nature and likelihood of the risks to key data. 

*Cryptography* is the field of study related to encoded information. *Encryption* converts plaintext to ciphertext and *decryption* does the reverse. *Substitution ciphers* substitute one character with another whereas, *transposition ciphers* rearranges the order of  characters in a message (e.g. route cipher). *Cryptanalysis* is the process of "breaking" a cryptographic code without a key. *Public-key cryptography* is where both users have a private and public key and this extends to use in digital signatures and digital certificates. 
