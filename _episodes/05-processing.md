---
title: "Processing ERPs data with EEGLAB"
teaching: 0
exercises: 0
questions:
- "How is data loaded into EEGLAB's EEG structure"
- "How can data be viewed from EEGLAB"
- "How can Event Related Potentials be generated in EEGLAB"
objectives:
- "Understand how to view and process data in EEGLAB"
keypoints:
- "Working with the data in EEGLAB"
---
## How to generate ERPs from an EEG recording using a basic procedure

#### **Import or Load a set file into EEGLAB**

![Matlab Integrated Development Environment]({{ page.root }}/fig/eeglab_load.png)
![Matlab Integrated Development Environment]({{ page.root }}/fig/eeglab_load_browse.png)

#### **Rereference to the average channel**

![Matlab Integrated Development Environment]({{ page.root }}/fig/eeglab_reref.png)
![Matlab Integrated Development Environment]({{ page.root }}/fig/eeglab_reref_pop.png)
![Matlab Integrated Development Environment]({{ page.root }}/fig/eeglab_rename_reref_pop.png)

#### **Filter the data**

![Matlab Integrated Development Environment]({{ page.root }}/fig/eeglab_filt.png)
#### **Parameters for the 1Hz high pass**
![Matlab Integrated Development Environment]({{ page.root }}/fig/eeglab_filt_hp1.png)
#### **Repeat for the 30Hz low pass**
![Matlab Integrated Development Environment]({{ page.root }}/fig/eeglab_filt_lp30.png)

#### **Remove bad channels**

![Matlab Integrated Development Environment]({{ page.root }}/fig/eeglab_rmch.png)
![Matlab Integrated Development Environment]({{ page.root }}/fig/eeglab_rmch_pop.png)
![Matlab Integrated Development Environment]({{ page.root }}/fig/eeglab_rmch_scroll.png)

#### **Rereference to the average channel**

![Matlab Integrated Development Environment]({{ page.root }}/fig/eeglab_reref.png)
![Matlab Integrated Development Environment]({{ page.root }}/fig/eeglab_reref_pop.png)
![Matlab Integrated Development Environment]({{ page.root }}/fig/eeglab_rename_reref_pop.png)

#### **Segment the data relative to face stimulus events**

![Matlab Integrated Development Environment]({{ page.root }}/fig/eeglab_epoch.png)
![Matlab Integrated Development Environment]({{ page.root }}/fig/eeglab_epoch_pop.png)
![Matlab Integrated Development Environment]({{ page.root }}/fig/eeglab_epoch_bl.png)

#### **Remove bad time segments (epochs)**

![Matlab Integrated Development Environment]({{ page.root }}/fig/eeglab_rmep.png)
![Matlab Integrated Development Environment]({{ page.root }}/fig/eeglab_rmep_pop.png)
![Matlab Integrated Development Environment]({{ page.root }}/fig/eeglab_rmep_scroll.png)
![Matlab Integrated Development Environment]({{ page.root }}/fig/eeglab_rmep_rej.png)

#### **save the segmented data**

![Matlab Integrated Development Environment]({{ page.root }}/fig/eeglab_save.png)
![Matlab Integrated Development Environment]({{ page.root }}/fig/eeglab_save_browse.png)

{% include links.md %}

