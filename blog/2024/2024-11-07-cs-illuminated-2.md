---
layout: post
title: Chapter 2
author: Arpon Sarker
date: 2024-11-07 10:13:00
categories: [technology, coding]
tags: [compsci, programming, algorithms]
---

# Computer Science Illuminated Chapter 2 - Binary Values and Number Systems

## Introduction
Before we can understand how computers represent information, we also must understand the number systems used and why they are used in the workings of a computing system. We need to understand this since this book opened my eyes to a fundamental definition of a computer. My definition has always been that a computation takes an input to an output from some algorithmic function but a much broader definition would be that a computer transforms data (as input) to some other representation (output).

## Positional Notation
A *number* is a unit belonging to an abstract mathematical system and is subject to the laws of succession, addition, and multiplication. Negative numbers and rational numbers are handled in the next chapter. 

*Positional Notation* was a huge step from counting with unique symbols for each kind of number such as 1 to 50 being 50 unique symbols, hence positional notation allows us to communicate much larger numbers with only 10 digits (assuming base 10, of course). This was emphasised by the invention of the abacus. For example, 943 can be represented as $9 \cdot 10^2 + 4 \cdot 10^1 + 3 \cdot 10^0$. The general formula is 
$$
d_n \cdot R^{n-1} + d_{n-1} \cdot R^{n-2} + \ldots + d_1 * R^0, \text{for base R, n digits and $d_i$ being the i-th position}
$$

To convert from some arbitrary base R to base 10 (decimal):
$$
d_n \cdot R^{n-1} \quad \ldots \text{same formula as above}
$$

To convert from base 10 to some arbitrary base R:
```
While (quotient != 0)
    Divide decimal number by new base
    Make remainder to the left of the answer
    Replace decimal number with quotient
```
Example (2748 to Hex):
$$
2748 \div 16 = 171 \cdot 16 + 12
\\
171 \div 16 = 10 \cdot 16 + 11
\\
10 \div 16 = 0 \cdot * 16 + 10
$$

Hence, the result is 10 11 12 which in Hexadecimal is **ABC**.

**Why does this Algorithm Work?**
$\\\text{Proof (using 2748/16)}:$
$$
2478_{10} = ABC_{16} \text{, as seen above}
\\
2748 = A \cdot 16^2 + B \cdot 16^1 + C \text{, this is in the form of D=nq+r}
$$
Hence, the digit C is the remainder in this equation and this is the exact method needed to be able to extract the least-most digit which in this case will be C by dividing by the base.
$$
\frac{2748}{16} = A \cdot 16 + B
\\
\frac{171}{16} = A
$$

## Powers of Two
Binary($2^1$), octal ($2^2$), and hexadecimal ($2^3$) all have a special relationship where a binary number can be easily converted to octal and hexadecimal and vice versa. To convert binary to octal, you group the binary digits from left to right in groups of three and that is the value of one octal digit. Of course, you may need to pad zeros on the right-most digits. To convert from octal to binary, you expand each octal digit into the equivalent binary representation which would take three digits.

*Example*
$$
1010110_2
\\
001 \quad 010 \quad 110
\\
126_8
$$

The same can be done for hexadecimal but instead of 3 digits it is 4.

**Why are computers in binary in  the first place?**

What was surprising to me was that the early computers were decimal machines or bi-quinary (2 switches with 5 switches for 0-4 and 5-9). However, nowadays all machines are in binary and this is the reason. 
We have Boolean algebra to thank for all the modern circuitry and conceptualisation for modern implementations, they use a low-voltage and a high-voltage signal which uses Pulse Code Modulation (PCM) to make sure a 0 is when the voltage is below a certain threshold, easier and cheaper to implement. For decimal systems, they had 10 different states for each transistor and 9 different thresholds which is much harder to control and is prone to signal degradation.

In the 1960s and 70s, the ENIAC, IBM 650, IBM 7070 all used decimal systems using either binary-coded decimal (BCD), bi-quinary and two-out-of-five code. [[1]](#1)

**Extra**: the $.$ is known as the radix-point and changes for each base it is written such as "*decimal point*" for base-10 or "*binary point*" for base-2.

8 bits are grouped into bytes and bytes are grouped into words (useful for showcasing the number of bytes a CPU can process at once and bus size such as 64 bit or 32 bit processors). The number of bits in a word is known as the word length. *half words* are 2 bytes, *full words* are 4 bytes, and *double words* are 8 bytes. 


## References
<a id="1">[1]</a> 
[Decimal Computer Wiki](https://en.wikipedia.org/wiki/Decimal_computer)
