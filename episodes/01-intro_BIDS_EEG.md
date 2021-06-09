---
title: "Introduction to EEG-BIDS"
teaching: 0
exercises: 0
questions:
- "Why are data standards important?"
- "What information needs to be standardized for EEG?"
objectives:
- "Understand the value of using data standards in research"
- "Understand the complexities of establishing a standard for EEG data"
keypoints:
- "What does it take to standardize an EEG project?"
- "What is gained by standardizing an EEG project?"
---

## The big picture of EEG data standards

#### **EEG data is complicated and with many properties that can be stored in an infinite number of ways**

In order to work with EEG data the researcher needs to work with several properties of the data. These properties include things like the voltage signals that are sampled at a specific rate, the physical locations of the recording sites, as well as more idiosyncratic properties like the experimental task event marks, etc. When building a lab or planning a new study decisions are made about all of the EEG properties and those properties make up the interpretable material of the research project. Decisions are also made about how all of that information is going to be stored so that it can be found and used by the researcher and software tools later.


#### **When a researcher is make decisions about EEG parameters and storage strategy for a lab or project some of the questions they might ask are:**

How should the information be stored so that it can be used efficiently now?

How should the information be stored so that it can be used efficiently later?

Could the data be efficiently shared with another research group?

Could another group or project's data be used or integrated (pooled)?

Is the data intended to be made open access and available long-term?

Are there existing analytic tools, procedures or platforms to which the data need to be compliant?

What are the costs now (and later) for designing a new unique data storage strategy?


#### **Can a data standard provide answers to these questions?**

It is always a concern that something important will be missed when designing a data strategy, a clear community driven discussion about adaptive best practices is an ideal way to build confidence in decisions.

The best way to keep data valuable in the long term is to have sufficient documentation that is accessible (both findable and interpretable) to not only yourself, but also to others in the future. A published standard offers this documentation not to mention various other resources (such as workshops like this one).

When sharing data that is compliant with a data standard the recipient only needs to become familiar with the standard in order to access the relevant properties and parameters of the research data.

Independent data sets that share compliance with a data standard can easily be pooled in terms of their storage strategy and access methods. Variance in project parameters still need to be addressed in the analytic process but those parameters can be accessed in common way.

Open-access data curation platforms are the ideal place to make a data project openly available over the long term. Compliance with a data standard greatly facilitates the injestion of data into databases or platforms.

Software and platform development often requires substantial effort for input and output diversity (or it is constrained to subset of data types). If a data standard has substantial uptake it is an ideal place for analytic tool developers to focus their attention.

People time in a research project is an important consideration and the time spent on designing a data management strategy can vary greatly. It is also important to note that a unique data management strategy can have unexpected cost in the future. An established data standard has had the oprotunity to collect experience from across the research community over several generations of projects. 

## **The face13 data set**

![face13 ICA decomposition]({{ page.root }}/fig/SDC_EEG_face13_ICA.png)

![face13 DAR decomposition]({{ page.root }}/fig/SDC_EEG_face13_DAR.png)

## **The EEG-IP-L (EEG Integrated Platform Lossless) processing pipeline**

![EEG-IP-L diagram]({{ page.root }}/fig/SDC_EEG-IP-L_diag.png)

![EEG-IP-L dashboard]({{ page.root }}/fig/SDC_EEG-IP-L_dash.png)

## **EEG-BIDS examples: face13 data and the EEG-IP-L derivative**

![BIDS examples root]({{ page.root }}/fig/SDC_EEG_BIDS_example.png)

![BIDS examples source]({{ page.root }}/fig/SDC_BIDS_example_sourcedata.png)

![BIDS examples raw]({{ page.root }}/fig/SDC_BIDS_example_raw_data.png)

![BIDS examples derivative]({{ page.root }}/fig/SDC_BIDS_example_derivative.png)

![BIDS examples derivative]({{ page.root }}/fig/SDC_BIDS_example_derivative_data.png)


{% include links.md %}

