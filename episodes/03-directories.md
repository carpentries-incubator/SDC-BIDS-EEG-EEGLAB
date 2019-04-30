---
title: "EEGLAB within BIDS-EEG"
teaching: 0
exercises: 0
questions:
- "What does EEGLAB need to know about the folder structures?"
- "How to set up the paths in Matlab/Octave"
objectives:
- "Undertand what EEGLAB needs to be able to find (data and scripts) and how to tell it where to find them."
keypoints:
- "Working with EEGLAB requires that specific files can be found in specific locations"
---

## What does Matlab/Octave need to know about the BIDS structure in order to run EEGLAB?

#### **EEGLAB is a set of Matlab functions (... which are text files).**

Before we get started analyzing EEG data in EEGLAB lets take a look at how the functions operate in the Matlab environment. Matlab is and interpreted language. This means that it will read some text, interpret it in a very specific way and then perform the operations that are defined by the text.

For our purposes we can think of Matlab doing two very important things:
1. it stores information in memory as different kinds of variables
2. it can perform operations (or functions) on those variable

Lets open the Matlab Integrated Development Environment (IDE) and take a look at these capabilities.

![Matlab Integrated Development Environment]({{ page.root }}/fig/matlabIDE.png)

> ## Note
> The Matlab IDE is made up of several sections in the Graphical User Interface (GUI). Each of these are important to understand as we move towards interacting with EEG data via EEGLAB.
> 1. Command Window: This is where we interact with Matlab using the Command Line Interface (CLI) creating variable and performaing operations on them.
> 2. Current FOlder: This is the directory that Matlab if pointing to. This is the part of the file system that Matlab sees an is its starting point for relative paths.
> 3. Workspace: this is a summary of the variables that are accessible to the Command Window
> 4. Command History: This is the interactive list of operations that have been called from the Command Window.
> 5. Editor: This is a text editor with added features for modifying Matlable interpreted text files (*.m files). 
>
> {: .source}
{: .callout}

#### **Creating variables in the Matlab CLI**
Making new variables (or modifying existing variables) is accomplished using the "=" character.

We can create a new variable named "x" and make it equal to a series of numbers:
'''bash
>> x=[1,2,3,4,5];
'''

We can also perform operations on the variable and have the result saved to a new varialbe "y":
'''bash
>> y=mean(x);
'''

{% include links.md %}

