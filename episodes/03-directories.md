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

#### **EEGLAB is a set of Matlab functions (... which are text files).

Before we get started analyzing EEG data in EEGLAB lets take a look at how the functions operate in the Matlab environment. Matlab is and interpreted language. This means that it will read some text, interpret it in a very specific way and then perform the operations that are defined by the text.

For our purposes we can think of Matlab doing two very important things:
1. it stores information in memory as different kinds of variables
2. it can perform operations (or functions) on those variable

lets open Matlab and take a look at these capabilities.

	![Matlab Integrated Development Environment]({{ page.root }}/fig/matlabIDE.png)
{% include links.md %}

