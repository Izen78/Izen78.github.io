---
layout: post
title: Chapter 1
author: Arpon Sarker
date: 2024-09-05 2:13:00
categories: [technology, coding]
tags: [compsci, programming, algorithms]
---

# Computer Science Illuminated Chapter 1

## Introduction
This blog is my first computer science blog and I wanted something with the breadth of the entire field to serve as an introduction.

Before getting into the first chapter, I think it's a good idea to understand the background of the book before actually delving inside the content. The authors of this book are John Lewis (born: 25/08/1963) from Virgina Tech. 
Funnily from his Wikipedia page [[1]](#1), his Twitter account is mistaken for others' identities ranging from a British Department store to the American politician and civil rights leader. At the time of writing this he is an adjunct professor at Virginia Tech but using 
the 3rd edition textbook from my university, it states he is at Villanova University. Nell Dale is the other co-author and is part of the IEEE Computer Society and was one of the first women to get a PhD in Computer Science in the 1970s and graduated and taught at the University of Texas, Austin.
Both of these authors have written extensively on programming languages for education and Lewis actively participates in the *ACM Special Interest Group on Computer Science Eduction* (SIGCSE) and Dale got an award from ACM SIGCSE in 1996.

## The Onion Layers
1. Information Layer
2. Hardware Layer
3. Programming Layer
4. Operating Systems Layer
5. Applications Layer
6. Communications Layer
![Layers of a Computing System](img/2024/cs-illuminated-layers.png)

The innermost layer - *Information Layer* - reflects the way information is represented on a computer. This is purely conceptual (using binary) and is used to represent a myriad of information types. 
The *Hardware Layer* includes devices such as gates and circuits which lead to CPU and memory. 
The *Programming Layer* deals with software, the instructions used to accomplish computations and manage data (in many forms and languages) to solve problems.
The *OS Layer* helps us interact with the computer system and manage how hardware, programs and data interact.
**These previous layers are for the computer system to work.** 
The *Applications Layer* focuses on solving specific real-world problems using domain-specific application programs. (AI, information systems and simulation)
The *Communication Layer* deals with connecting computers to networks and how they share information and resources.

## Laying the Groundwork
The start of the book goes into **The Big Picture** and defines a "Computing System" as the hardware, software and data to solve problems.

## Abstraction 
The levels discussed above are examples of abstraction - *a mental model which removes or hides complex details*. Human beings can actively manage about 7 $\pm$ 2 pieces of information in short-term memory at one time (**Miller's Law**).
7 is seen as a small number but with abstraction can represent a chunk of information for each slot.

## History of Computing
### History of Hardware (From abacus to UNIVAC)
- In early history times, people believed that the *Stonehenge* is an early form of calendar/astrological calculator. 
-The *abacus* ($16^{th}$ century BC) was developed fo record numeric values to perform basic arithmetic.
- *Blaise Pascal*, in the middle of the $17^{th}$ century built and sold gear-driven mechanical machines which performed integer addition and subtraction.
- Later in the same century, *Gottfried Wilhelm von Leibniz* built the first device designed for all 4 operations. It wasn't very reliable.
- *Jacquard's Loom* developed by Joseph Jacquard used a series of cards with punched holes and though not a computing device - was the first to use input.
- *Charles Babbage* designed the *Analytical Engine* which was never implemented but utilised memory, both numbers and mechanicals steps using punch cards.
- *Ada Augusta, Countess of Lovelace* extended and corrected Babbage's work, becoming the world's first programmer. The created the concept of a loop and has a language Ada (US D.o.D.)named after her.
- *William Burroughs* produced and sold a mechanical adding machine.
- *Dr. Herman Hollerith* developed the first electro-mechanical tabulator (revolutionizing the census) and later formed IBM.
- In 1936, *Alan Turing* invented an abstract mathematical model, the Turing machine.
- From WWII, the *Harvard Mark I* and the *ENIAC* are two of the more famous machines. *John von Neumann* was a consultant on the ENIAC project and started working on the *EDVAC* which was completed in 1950. 
- The *UNIVAC I* after was the first computer used to predict the outcome of a presidential election.

**First Generation (1951-1959):**
Commercial computers used vacuum tubes, generated a great deal of heat and was not reliable and required large specially-built rooms. The primary memory device was a *magnetic drum*. The input device was a card reader (descendant of Hollerith card). The output was either a punch card or line printer. By the end of this generation, magnetic tape drives had been developed.
Storage devices external to the computer memory are called *auxiliary devices*.

**Second Generation (1959-1965):**
The *transistor!* (which won a nobel prize). The memory used were *magnetic cores* and a new auxiliary device developed was *the magnetic disk*.

**Third Generation (1965-1971):** 
*Printed ciruit boards* were used in the previous generation. This generation was characterized by *Integrated Circuits* (IC). Moore's Law also came to be from Gordon Moore (co-founder of Intel).
Integrated-circuit technology allowed memory boards to be built by transistors but auxiliary storage devices were still needed as the information was wiped when the power went off.

**Fourth Generation (1971-?):**
*Large-scale Integration*  meant moving from several thousand transistors on a silicon chip to a whole microcomputer by the middle of the decade. The phrase *Personal Computer* (PC) had also been entered into the mainstream.
Apple, Hewlett-Packard, IBM, NCR, Remington Rand, DEC, Control Data and Burroughs...
The introduction of the RISC architecture and machine language and Sun Microsystems introduced a RISC chip on a workstation or UNIX workstations.
Moore's Law had also changed to: "Computers will either double in power at the same price or halve in cost for the same power every 18 months"

Parallel computing was introduced in the late 1980s and relied on parallel architectures on a set of interconnected CPUs either SIMD or MIMD.
Networking in the 1980s involved the invention of *The Ethernet* and its protocols and in 1979 DEC, Intel and Xerox made it a standard.
By 1989, PCs were connected together with a file server and LANs also came to be known.
The internet descended from *ARPANET* a government-sponsored network started in the late 1960s and uses packet switching.

### History of Software

**First Generation (1951-1959):**
The first programs were written using *machine language*.

## Computing as a tool and discipline

## References
<a id="1">[1]</a> 
[Wikipedia Page](https://en.wikipedia.org/wiki/John_Lewis_(computer_scientist))
