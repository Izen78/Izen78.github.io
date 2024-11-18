---
layout: post
title: Chapter 7
author: Arpon Sarker
date: 2024-11-18 20:38:20
categories: [technology, coding]
tags: [compsci, programming, algorithms]
---

# Computer Science Illuminated Chapter 7 - Low-Level Programming Languages

## Introduction
The operations a computer can perform are in its definition it is *programmable*, and able to *store*, *retrieve*, and *process*. 

## Machine Language
Remember from before these instructions are literally built into the circuits for the device to recognise specific bit commands devised by them. Here we use Pep/7's CPU which contains a PC, IR, accumulator (A register), status bit N (1 if negative), and status bit Z (1 if zero). The entire instruction format is 24 bits - 8 bits for the instruction specifier and (optionally) 16 bits for an operand specifier. The instruction specifier is made up of several sections: the operations code is 5 bits long and specifies which instruction is to be executed ($2^5$ instructions), a register specifier of 1-bit which is always 0 since we are just using the A register, and a 2-bit addressing mode specifier where 00 is immediate mode where the operand is a 16-bit integer and if 01 it's direct mode where the last rightmost 12 bits is a memory address. 

## Assembly Languages
Assembly languages assign mnemonic letter codes to each machine-language instruction. A program called an *assembler* reads each of the instructions in mnemonic form and translates into its machine-language equivalent. Because of each type of computer has a different machine language, there are as many assembly languages and translators as there are types of machines. The code is written in hexadecimal and the addressing mode is specified alongside this. Pseudo-operations are *assembler directives* or instructions to the translating program which assigns blocks, words etc. This is done first and then the code is executed. Branches and jump statements can be used for flow control for both selection and iteration. There is still abstraction here where Pep/7 uses 2's complement to represent negative numbers and can specify decimal numbers (e.g. d#25) and setting up blocks of storage. 

