---
title: Week one
date: 2020-08-03 07:42:34
slug: week-one
---

## Input/Output

> **Context**
> Before writing this, I had completed the week 0 lecture from Harvard’s CS50: Intro to Computer Science.

A useful place to start is to understand what computers actually do. At their simplest, the core job performed by a computer is to simply take a set of instructions, execute the steps and return the result of this execution. The instructions, steps, directions that we give a computer is known as the **input**. The outcome of the processing, compilation, analysis, execution is what is known as the **output**. And that’s all a computer does! Takes a set of inputs, processes them and gives us an output. It’s extremely efficient at this job. The role of the computer programmer is to codify how the computer should process this input to give the expected output. So whether it’s the maths to add two numbers together, the analysis you viewing habits to produce some Netflix recommendations or an Instagram filter to make your photos look better - a person (or a group of people) have programed a computer to take these input, process them in a particular way, and produce an output … and hopefully your pictures look better for it!

## Binary

We’ve established - at a simple level - what a computer does. Now, let’s look at how it does this. Computers talk in binary. Whereas, humans tend to communicate in denary, which is a fancy term for a decimals. A denary number system has a base of 10, which means we have 10 digits that we can use.

`0 1 2 3 4 5 6 7 8 9`

Obviously, we can count higher than 9, but higher numbers are just a combination of these existing numbers. For example:

`19 250 1000 123456 12972457257450970607357906730953`

The biggest numbers possible are simply a different combination of one of the 10 available digits. In contrast, binary is a number system with a base of 2. Therefore, rather than the 10 digits available in a denary (or decimal) system, binary only has 2 available digits: `0` and `1`. For example, to express a number like 168 in binary, we would write:

`10101000 => 168 in denary`

Okay, let’s count to 10 in binary. Do you notice any pattern?

```
0 // 0
1 // 1
10 // 2
11 // 3
100 // 4
101 // 5
110 // 6
111 // 7
1000 // 8
1001 // 9
1010 // 10
```

As we see, similar to our denary system, we can create different numbers by combining ones and zeros in different orders. Binary actually has similarities to our denary number system. For the `15` in our denary system, we would split this number out into 1s, 10s and 100s.

```
100 10  1
 0  1   5
```

The important point is each place for a digit represents a power of ten because the denary system has a base of 10. For bigger numbers like `52743` - we can go further and count the thousands and ten thousands, but the steps alway increase by a power of ten.

```
10000 1000 100 10  1
  5    2    7   4  3
```

Therefore, if a denary - a number system with a base of 10 - increases each place value by a power of 10, how does binary work? We know binary has a base of 2, so we would expect each place value by a power of 2. So our steps - our equivalent to 1s, 10s, 100s, 1000s - would increment by the power of 2 each time.

```
8 4 2 1
? ? ? ?
```

Now, we just need to fill in the blanks. We are working in binary now, so we can only fill the blanks with a `0` or a `1`, so if we wanted to represent the number 4 in binary we would do so by writing `100`. Each one of these zeros and ones is known as a binary digit or a bit.

```
4 2 1
1 0 0
```

To do bigger numbers, we can go further… What would this equal?

```
128 64 32 16 8 4 2 1
 1  1  1  1  1 1 1 1
```

That’s right - 255! We can store up to 8 bits, which is known as a byte, so this means 255 is the maximum number we can make out of one byte. Computers use bits as the fundamental building block of their architecture. You may have heard references to bits such as 32-bit edition or 64-bit edition - this can mean computers will process 32 bits or 4 bytes at a time. This simply refers to the speed at which computers or programs can process bits or data (stored as bits). A computer takes an input, convert it into bits and process it to give an output.

We’ve looked at the role of a computer - processing an input into an output - and how using binary it achieves this goal. I suppose a lingering question is why? Why does it use binary to process an input into an output? Fundamentally, a computer internally is just made of millions of switches (or transistors) that can store electricity. Electricity only has two states: on or off. As a result, this lends itself perfectly to binary because we have seen binary has only two states: `0` and `1`. Therefore, a `0` could represent an off state and `1` can represent an on state. And because we are working with binary, we can be confident that there will not be any other options or outputs. This is a major benefit of binary.

## Project

> **Context**
> Before writing this, I had completed the week 0 lecture from Harvard’s CS50: Intro to Computer Science.

The second half of the lecture covers pseudocode and general programming concepts like variables, booleans, conditional statements and the basic building blocks of a coding language. I haven’t focused too much on this because, with a background of web development, this was fairly basic information (and I assume most of the readers of this post will be familiar with at least one programming language).

A chunk of the first lecture also contains an explanation of the program Scratch - a MIT developed, user friendly GUI - which has many of the basic constructs of programming. Again, I haven’t documented much on this as it is more about the practical use of the platform. The video lecture gives you all you need to know - so there isn’t much that I can add.

## Problem

The problem set for week one was to build your own game in Scratch, which must meet certain requirements. Once you get the hang of how the scratch interface functions, you can get a game up and running pretty quickly. The requirements that must be met are:

- Your project must have at least two sprites, at least one of which must resemble something other than a cat
- Your project must have at least three scripts total (i.e., not necessarily three per sprite)
- Your project must use at least one condition, one loop, and one variable
- Your project must use at least one sound

I must admit, I didn’t spend a massive amount of time on this project because I just wanted to get into the substance of the course. However, I did create a game which passes the requirements. If you have or intend to purchase a certification with the course, then completing this project is required.
My idea came from a game called ![Sprinter](https://www.gamedesign.jp/flash/sprinter/sprinter.html), which was an old flash browser-based game. The game was simply a 100m race against the computer, which requires you to press the left and right arrow keys alternately as quickly as possible to increase your running speed. The catch was that if the arrow keys were not pressed alternately - because you lost your rhythm - you would go slower and would risk falling over. The game was simple, but highly addictive. This my effort to recreate it in Scratch.

<iframe src="https://scratch.mit.edu/projects/287370691/embed" allowtransparency="true" width="100%" height="402" frameborder="0" scrolling="no" allowfullscreen></iframe>

## Further Reading

- [Lecture notes - week 0](https://cs50.harvard.edu/x/2020/notes/0/)
- [Binary representations in digital logic](https://www.geeksforgeeks.org/binary-representations-in-digital-logic/)
- [Bits, bytes, building with binary](https://medium.com/basecs/bits-bytes-building-with-binary-13cb4289aafa)
- [Khan Academy: Bits and Bytes](https://www.khanacademy.org/computing/ap-computer-science-principles/x2d2f703b37b450a3:digital-information/x2d2f703b37b450a3:bits-and-bytes/a/digital-data-introduction)
- [Number system and base conversions](https://www.geeksforgeeks.org/number-system-and-base-conversions/)
- [Conversion tables](https://www.prepressure.com/library/technology/ascii-binary-hex)
- [Hex and other magical numbers](https://medium.com/basecs/hexs-and-other-magical-numbers-9785bc26b7ee)
