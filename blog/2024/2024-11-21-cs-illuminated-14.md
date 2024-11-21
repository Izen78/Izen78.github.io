---
layout: post
title: Chapter 14
author: Arpon Sarker
date: 2024-11-21 12:17:50
categories: [technology, coding]
tags: [compsci, programming, algorithms]
---

# Computer Science Illuminated Chapter 14 - Simulation, Graphics, and Other Applications

## Introduction
Here we look at the theory behind computer simulations and cover many more applications software such as computer graphics, embedded systems, e-commerce, and computer security.

## Simulation
*Simulation* is developing a model of a *complex system* and experimenting with the model to observe the results. A *system* is defined as a collection of objects interacting in some way such as a collection of hardware and software to form a computing system. A *complex system* is a system best suited for simulation that is characterised as dynamic, interactive, and complicated. A *model* is an abstraction of a real system; a representation of objects within a system and the rules that govern the behaviour of the objects. Hence, a *simulation* is developing the rules and behaviours of a collection of interacting objects. We look at logical simulations (represented in a computer program), not purely physical (wind tunnel) or combination of physical and software control (flight simulator). 

To construct models, requires identifying a small subset of characteristics/features that are sufficient to describe the behaviour. The distinction between the two types of model is based on how time is represented: as a continuous variable or discrete event.

### Continuous Simulation
A continuous simulation treats time as continuous and express changes in terms of a set of differential equations. Thus, the behavours of the models are ones that are understood by a mathematical definition which are the characteristics/features of the model. For example, meteorological modelling falls into this category.

### Discrete-Event Simulation
These models are made up of *entities*, *attributes*, and *events*. An entity represents some object, The characteristic/feature of the system is an object. An attribute is a characteristic of an entity and an event is an interaction between entities. An entity can also represent a resource that other entities need and can wait on (such as cashiers for bank model). Pareto's law says that 80% of the behaviour is from 20% of the components. You can already see it is quite easy to implement this with object-oriented design where the object classes are the entities, attributes are class properties/fields, and events are the responsibilities or the rules defining class interactions. For instance, a queuing system is an example of this model.


## Computer Graphics
Computer graphics play a role everywhere in computer science such as the GUI of operating systems, word processors and desktop publishing software are examples of application software that still require computer graphics to draw to a screen, illustrations on a computer, and computer-aided design (CAD). The most "fun" applications which are computer games, animated films, or special effects in movies are the most complex. 

Our visual system works by light reflecting off objects and entering our eyes. The lens of the eye focuses the light as it strikes to the back of our eye. The back of the eye is composed of cone and rod cells where cone cells come in 3 varieties (long-red, middle-green, short-blue) and rod cells which only react to intensity of light, lacking colour sensitivity. In addition to the reflection of light, the appearance of this reflection is based on the object's composition such as the way their particles are structured where plastic is much more shiny due to its embedded colour particles but wood reflects light unevenly giving a lesser intensity in the reflection.

Shapes also matter where the normal vector which is perpendicular to the surface can be by itself in a flat object or multiple in a more complex shape (not flat). This can alter the highlight shape, giving us cues as to the shape of the object. We use equations to describe many mathematical objects but this isn't enough to cover all real world objects and requires describing the shape of curved surfaces and defining complex objects as individual curves. 

To simulate light, the *illumination model* is the simulation of light on **one** point of an object. The *shading model* is using the illumination model for the **entire object**. The process of creating an **entire image** is *rendering*. One of the earliest illumination models uses three different components: ambient light, diffuse reflections, and specular reflections and combines them all but makes everything look plastic (fixed with textures) and cannot handle transparent objects or objects with mirror-like surfaces. The second shading method is to use *ray tracing* which a point in space is identfied where the viewer and the location of the screen is located. Lines can be drawn from the viewer to each pixel location of the image where it is followed and when it hits something changes pixel colour. This also handles transparent and reflective objects. *Radiosity* is to handle colour bleeding where colour reflects of an object onto another (like a red shirt next to a white wall). Radiosity treats light as energy calculates how much energy is transferred from every object to every other object.

For modelling complex object, we look at midpoint subdivision for creating fractal terrains. Plant growth can be modeled through both grammar (rules in English grammar specify how components of a plant change) and probabilistic methods. Liquids, clouds, smoke and fire haved equations developed that *approximate* the behaviour of liquids, gases, and fire. 

Animated films and movie special effects always looks better than video games since they don't have to generate images in real-time. 

## Embedded Systems
*Embedded systems* are computers that are designed to perform a narrow range of functions as part of a larger system. An embedded system is typically on a single microprocessor chip with the programs stored in ROM. We use assembly as C is 25% larger and slower  where size of the ROM is of primary concern.

## E-Commerce
Electronic commerce is the process of buying and selling products and services using the World Wide Web. Somehow, the "dot-com" collapse of 2001, instead of diminishing e-commerce actuall made the way for organisations with legitimate business models. The challenges here are security which is divulged in the next section.

## Computer Security
We have already visited computer security which can be said to have its own onion layers or abstractions. For instance, the OS must protect application programs from accessing other programs or the OS in main memory as well as file permissions in a multiuser system. For the security of information itself, we talked about cryptography. Other aspects of security are *authentication credentials* which is the information a user provides to identify themselves for computer access. A *smart card* which a card with an embedded memory chip used to identify users and control access could be used as well as *biometrics* which is using human characteristics to identify users and control access. These last two approaches are more expensive and biometrics can be prone to false rejections and false acceptances. 

*Malicious code* can be defined as any program that explicitly attempts to bypass appropriate authorisation and/or perform unauthorised functions. A *virus* is a malicious, self-replicating program that embeds itself into other code. A *worm* is a malicious stand-alone program that often targets network resources. A *Trojan horse* is a malicious program disguised as a benevolent resource. A *logic bomb* is a malicious program that is set up to execute when a specific system event occurs. *Password guessing* is an attempt to gain access by methodically trying to determine a user's password and *phishing* which is using a web page to masqueade as an authoritative system and trick users into revealing security information are forms of *spoofing* where a malicious user masquerades as an authorised user. A *back door* is a program feature that gives special and unauthorised access to a computer system to anyone who knows it exists. *Buffer overflow* is a defect in a computer program that could cause a system crash and leave the user with heightened privileges. A *Denial-of-service* (DoS) is an attack on a network resource that prevents users from accessing the system. Lastly, *man-in-the-middle* is where the network communication is intercepted in an attempt to obtain key data (mitigated through cryptography). 
