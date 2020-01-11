---
title: "Programming Isn’t for Everybody"
categories:
  - blog
tags: 
  - programming
  - advice
---


**I was at a training event** related to the AT&T Developer Program a little while back. We were one of a series of groups who were given these nifty little credit card-sized Texas Instruments LaunchPad computers and they were running us through the process of uploading code onto them and executing it.

Working with embedded systems like the LaunchPad, where you’re presented with a CPU (in this case a 32-bit ARM Cortex–M4F) and a bunch of discrete components with some glue code so they can communicate, you’re programming “close to the metal,” and if one small step in the sequence is slightly off the whole thing may hang and never respond again. This is a case where turning the problem machine off and back on again is definitely a viable strategy to fix problems!

More people than expected were in attendance, so I was sitting on a couch in an overflow room where the trainer was mostly audible and visuals partly visible, following an example procedure in the written materials when the output from the computer froze. As I unplugged the LaunchPad from the laptop to reset it and started rebooting and connecting to the development environment, I turned to the person next to me on the couch to see if he was any further along than I.

Alas, such was not the case, and he was feeling like he had run into a brick wall following the instructions. He would simply have to start again without knowing what had gone wrong and hope the result would be different. I asked if he was a programmer, and he said no, he was in marketing. I told him, “The next time someone tells you that everyone must program, remember this moment.”

- - -

**Programming computers**, like any other professional trade or substantial body of knowledge, is difficult to learn. To use the ever-popular car analogy, most people would just like their car to take them places and not have to fiddle with the engine. There are very few things on a car that your average person could fix without professional help. Computers, like cars, are technological enablers, and though someone with expert skills can do amazing things with them, most folks are content with the basics (communication, social connection, entertainment) and more or less leave the creativity to others.

And computers are becoming more difficult to understand than ever, even for pros. Modern consumer OSes have hundreds of thousands of system calls that can be made, far too many to memorize or even be entirely familiar with. We may behave as though our code is the dominant force operating but in fact it’s constantly being swapped in and out of working memory at gigahertz speeds as the computer is doing a dozen other things including updating screen widgets like clocks and other background processes like networking, disk transfers and memory management.

For that matter there are fundamental parts of the computer the even the people who write the OS and design the hardware don’t have access to. The CPU may have boot code written in an entirely separate and undocumented language. The keyboard has its own dedicated processor. Your smartphone has a whole parallel operating system to run the onboard radio transceiver that communicates with the cellular network and makes your phone calls possible — even manufacturers like Apple or Samsung who design their own processors use someone else’s chips for this. (The potential for security failure is very real in these areas, and virus scanners don’t check them. If one of these gets infected there is currently no cure short of junking the device.)

- - -

**I do think most folks** would benefit from learning a little programming at an early age. Developing a concept of what an algorithm is and how it is executed step by step like a recipe, having an idea of how a general-purpose processor operates, understanding the basics of how a web page is made and served over a network — these should be part of basic cultural literacy.
{: .notice}

And those of us who excel in all this, no more than 10% of the population I’d imagine, would be introduced to the joys (and perils) of programming at an age when brains are still developing, potentially encoding in hardware the kind of logic, fidelity to facts, and capacity to assimilate and act on very large aggregates of information that — let’s face it — our species needs to continue to operate a worldwide industrial civilization without making the planet uninhabitable.
