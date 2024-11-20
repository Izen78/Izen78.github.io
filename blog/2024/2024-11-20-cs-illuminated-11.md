---
layout: post
title: Chapter 11
author: Arpon Sarker
date: 2024-11-20 14:42:17
categories: [technology, coding]
tags: [compsci, programming, algorithms]
---

# Computer Science Illuminated Chapter 11 - File Systems and Directories

## Introduction
Second memory is nonvolatile and makes way for data used primarily for archival purposes. File systems and directories are the organisational methods for the various types of data.

## File Systems
A *file* is a named collection of related data. A *file system* is the logical view that an OS provides so that users can manage data as a collection of files. A file system is often organised by grouping files into *directories*. All files are either text files (containing bits interpreted as character sets) or binary files (bits are interpreted in some special representation). Eext files of a high-level language are called *source files*. For other information types, special programs must be set up or modified to view/modify a specific type of binary file. Files that are usually thought of as text files might not be due to the inclusion of font, margins, headings, colours, and images as additional information stored. File types are the specific kind of information in a file (denoted by its extension). 

To access a file, there is *sequential access* where data in a file is accessed in linear fashion by moving the current file pointer accordingly and *direct file access* is where data in a file is accessed directly, by specifying logical record numbers.

For file protection, there is an *owner* (creator of the file) with the highest permissions which can delegate some of these permissions to assorted group members in a *group*. The *world* is the rest of the users that have access to this multiuser system and usually have no or minimal privileges.

## Directories
A directory in an OS is most often represented as a file which contains data about the files inside it such as name, file type, address on disk, current size, protections, first created, and last modified. *Directory trees* are a structure showing the nested directory organisation of the file system. *Root directory* is the topmost directory where all others are contained in itself. The current *working directory* is the currently active subdirectory. For *paths* which are a text designation of the location of a file or subdirectory, they can be *absolute paths* which start from the root or *relative paths* which start at the current working directory. The paths can end in a subdirectory or a file itself. The **PATH** OS variable allows the user to specify a set of paths that are searched to help resolve references to executable programs where no matter what working directory you are in you can type "code" for VSCode.

## Disk Scheduling
The most important hardware device used as second memory is the magnetic disk drive. However, transferring data to and from secondary memory is the worst bottleneck and is the **slowest** part of the computer. *Disk scheduling* decides which outstanding requests for disk I/O to satisfy first. *Seek time* is the amount of time it takes for the heads to reach the appropriate cylinder and *latency* is the additional time it takes for the platter to rotate into proper position. Seek time is the most restrictive and is the primary issue dealt with here. 
- First-Come, First-Served: process the requests in the order they arrive, but passes over shorter distance cylinders 
- Shortest-Seek-Time-First (SSTF): moves the heads the minimum amount necessary, *starvation* may occur where earlier requests aren't satisfied since the later requests are always at a shorter distance.
- SCAN: works the same as elevators - moves towards the spindle and out towards the platter edge and so forth and starvation cannot occur since each cylinder is processed in turn. (variants: Circular SCAN, LOOK)
